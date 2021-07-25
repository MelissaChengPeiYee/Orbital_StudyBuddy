# **Orbital 2021 Developer Guide** 

## Team Study Buddy 

* [**Orbital 2021 Developer Guide** ](#orbital-2021-developer-guide)
    * [Team Study Buddy](#team-study-buddy)
        * [1. System Design](#1-system-design)
            * [1.1 Main Design](#11-main-design)
            * [1.2 Relevant Tools](#12-relevant-tools)
            * [1.3 Installation](#13-installation)
        * [2. Basic app flow](#2-app-flow)
            * [2.1 User Flow](#21-user-flow)
            * [2.2 Basic System Flow(Authentication)](#22-system-flowauthentication)
                * [2.21 Sign up System Flow](#221-sign-up-system-flow)
                    * [2.211 Data updates to Firebase Firestore](#2211-data-updates-to-firebase-firestore)
                * [2.22 Log in System Flow](#222-log-in-system-flow)
          
        * [3. Implementation](#3-implementation)
            * [3.1 Create study group Feature](#31-create-study-group-feature)
                * [3.11 Data Updates to Firebase Firestore](#311-data-updates-to-firebase-firestore)
            * [3.2 Join study group Feature](#32-join-study-group-feature)
                * [3.21 Displaying Study Group Lists](#321-rendering-study-group-lists)
                * [3.22 Join Group Flow](#322-join-group-flow)
                * [3.23 Data updates to Firebase Firestore](#323-data-updates-to-firebase-firestore)
            * [3.3 View study group Feature ](#33-view-study-group-feature)
                * [3.31 Displaying user's study group lists](#331-displaying-users-study-group-lists)
                * [3.32 Displaying additional ZOOM Meeting details](#332-displaying-additional-zoom-meeting-details)
            * [3.4 Chat Feature](#34-chat-feature)
    
        * [4. Testing](#4-testing)
            * [4.1 System Testing](#41-system-testing)
            * [4.2 User Testing](#42-user-testing)


### 1. System Design

#### 1.1 Main Design
Comes in the form of an out of the box mobile application.

Allows user to easily create and join study group sessions. All details are rendered through React Native Flatlist.

Largely supported by Firebase, with its main role as 'backend'.

All study group details are stored within the Firestore database, same for user accounts and their customized profiles.

#### 1.2 Relevant Tools

Our project will use a number of languages and libraries:

- JavaScript, ES6
- Firebase
- React Native
- React Navigation
- React Native Safe Area Context
- Redux
- React-redux
- React Native Async Storage
- React Native Paper
- React Native Community / Datetimepicker
- Moment
- React Native Picker
- React Native Vector Icons
- React Native Tab View
- React Native Gifted Chat
- React Native Webview
- React Native Document Picker
- Expo Image Picker
- Expo Document Picker
- React Native Search Bar
 
 #### 1.3 Installation
 Developers with git can clone this repository to obtain a copy of the source code:

```git clone https://github.com/MelissaChengPeiYee/Orbital_StudyBuddy```

We recommend using the IDE [Visual Studio Code](https://code.visualstudio.com/) to run our source code as it is versatile and can run Javascript files.

Developers can then do ```yarn install``` to download the node modules.

Once done, you are free to develop anything on the app. Happy journey ahead!

### 2. App flow

#### 2.1 User Flow

<img src = "https://i.ibb.co/zRsJ3sL/Untitled.png" width = "600" height = "500"/>

#### 2.2 System Flow(Authentication)

##### 2.21 Sign Up System Flow

<img src = "https://i.ibb.co/xHRHJrj/Untitled-1-1.png" width = "500" height = "300"/>

###### 2.211 Data updates to Firebase Firestore

*  Under the ```Users``` Collection, a new user id will be randomly generated. The new document id will be the new user id generated randomly by Firestore, representing the new user. <br><br>The document consists of the following fields: <br><br>
```uid``` the id of the user  <br><br>
```email``` the new user's email<br><br>
```password``` the new user's password <br><br>
```userName``` the new user's username  <br><br>
```profilePic``` the new user's profile picture, for first time user, it will be set as the Study Buddy logo by default <br><br>
```coverPic``` the new user's cover picture<br><br>
```groups``` an array consists of the group ids of the groups that the user has joined or created. At the point of creating an account, it should be empty. <br><br>


##### 2.22 Log In System Flow
<img src = "https://i.ibb.co/XF71WqS/Untitled-2.png" width = "500" height = "300"/>

### 3. Implementation

#### 3.1 Create study group feature

<img src = "https://i.ibb.co/92f05xK/Untitled-3.png" width = "500" height = "500"/>

##### 3.11 Data updates to Firebase Firestore

Under  ```api/dataServices``` , the  ```createGroup``` function updates the following fields on Firestore database:

* Under the ```Users``` Collection, followed by user ids as document ids, there is a field named ```Groups``` which consists of an array of group ids, which are the study groups that the user has created or joined. Upon creating a study group, Firestore will generate a unique id for that particular study group.
Then, the new group id will be added to the ```Groups``` array under ```Users``` Collection on Firestore.

* ** Under the ```Group``` Collection, a new document will be generated. The new document id will be the new group id generated randomly by Firestore, representing the new group created by the user. <br><br>The document consists of the following fields: <br><br>
```uid``` the id of the user creating the study group, aka the host's id <br><br>
```id``` the study group id <br><br>
```meetingDate``` the group's meeting date <br><br>
```startTime``` the group's meeting starting time <br><br>
```endTime``` the group's meeting end time <br><br>
```memberNo``` the maximum number of participants for the study group, this is a fixed number set by the host <br><br>
```members``` an array consists of user ids which are the users of the study groups, including the host <br><br>
```module```  the group name <br><br>
```zoomCode```  zoom code <br><br>
```zoomLink```  zoom link<br><br>
```zoomPassword```  zoom password<br><br>
```vacancy``` the no of vacancy of the study group, reduces by one every time someone join the study group or the host creates the study group<br><br>
```available``` the availability of the study group, if reached max capacity, then becomes unavailable<br><br>

Upon creating a study group, the field ```vacancy``` reduces by one. All other fields will be updated to what the host has key-ed in.



* ** The same applies to the ```Groups``` Collection, however the ```Groups``` Collection consists one additional ```Chats``` subcollection for storing chat details within each study groups.


#### 3.2 Join study group feature

##### 3.21 Rendering study group lists
Under  ```api/dataServices``` , the  ```getOtherGroups``` function is in charge of rendering a flat list of groups for the users to join. It filters out the groups which the user has already joined or created as well as the groups that are no longer available (maximum pax reached), and display according to the ascending order of the study group meeting date. If the user wants to display by module name, he/she can utilize the search bar filter function. 


##### 3.22 Join Group Flow

<img src = "https://i.ibb.co/rtrJBky/Untitled-5.png" width = "300" height = "300"/>

##### 3.23 Data updates to Firebase Firestore

Under  ```api/dataServices``` , the  ```joinGroup``` function updates the following fields on Firestore database:

* Under the ```Users``` Collection, followed by user ids as document ids, there is a field named ```Groups``` which consists of an array of group ids, which are the study groups that the user has created or joined.
Upon joining, the new group id will be added to the ```Groups``` array under ```Users``` Collection on Firestore.

* ** Under the ```Group``` Collection, followed by each unique group ids as document ids, there is a field named ```members``` which consists of an array of user ids, which are the members of that study group.
Upon joining, the new user id, which represents the user, will be added to the ```members``` array under ```Group``` Collection on Firestore.
Also, the field ```vacancy``` also reduces by one.
If the field ```vacancy``` becomes 1, the field ```available``` will be set to false.

* ** The same applies to the ```Groups``` Collection.

#### 3.3 View study group feature

##### 3.31 Displaying user's study group lists
Under  ```api/dataServices``` , the  ```getGroups``` function is in charge of rendering a flat list of groups that the users has joined or created themselves. 

##### 3.32 Displaying additional ZOOM Meeting details

Under  ```api/dataServices``` , the  ```getGroupData``` function is in charge of displaying additional group meeting details.

#### 3.4 Chat Feature

Under the ```Groups``` Collection, followed by each unique group ids as document ids, there is a subcollection named ```Chats``` which stores each group's chat details. 
Under the ```Chats``` subcollection, whenever a user sends a message, a unique id is randomly generated as document id, along with the following fields: <br><br>
```_id``` the text document id <br><br>
```createdAt``` the timestamp at which the text is send <br><br>
```text``` the message <br><br>
```user``` the sender which consists of two nested fields : ```_id``` the sender's id & ```name``` the sender's username <br><br>

### 4. Testing

#### 4.1 System Testing

#### 4.2 User Testing
We conducted a survey through Google Forms which can be found [here](https://docs.google.com/forms/d/e/1FAIpQLSc8kXDYUngq85MD3wxsAuGCM_vyHuFQ2f8aqOYG8_ESHkUoug/viewform?usp=sf_link).

The survey included a small task list for participants to attempt and try. They include the main functionalities of our extension.

You can also find the questions and results of our surveys [here](https://github.com/MelissaChengPeiYee/Orbital_StudyBuddy/blob/main/doc/UserTesting.md).





