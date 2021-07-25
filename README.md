<article>
  <header>
    <h1>Study Buddy - Your complete online study platform</h1>
  </header>
</article>
<img src="https://i.pinimg.com/originals/a8/40/25/a840257675efeda45326e763e1ff451e.jpg" alt="Girl in a jacket" width="800" height="500">
<h2>Motivation</h2>
Have you ever felt unmotivated to study for a module or perhaps in the process of revising course materials, you bump into a question and are seeking immediate response to your queries? Obviously your TAs and lecturers won’t be available 24/7 to attend to your questions, so a study group might just be what you need!
 
 <br> Forming a physical study group isn’t easy given social distancing restrictions nowadays, and finding a perfect spot for it can sometimes be troubling. With the advent of a virtual study group app, you can stay at your own place and have an informative discussion with your course mates, at anywhere, anytime. <br>
 
However, here comes the problem. How can you search for course mates with the same need as you? You can’t just approach and ask every single one you met, let alone comparing each other's schedule and agree on a timeslot. Especially with COVID, you may not even get a chance to meet your module-mates in person. The time you spent to find a whole bunch of suitable study group mates may be used for more meaningful stuff. Therefore, a platform which enables one to create or join a study group according to their available time might just come in handy.

<h2>Aim</h2>

We hope to be able to provide users with a platform for them to participate in different study sessions for their own benefit. Here, they will be able to join different groups according to their preferred time slots. Additional features are tailor-made to ensure that their user experience is enhanced to the maximum.

<h2> User Stories </h2>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">General Activity</th>
    <th class="tg-0pky">General User Task</th>
    <th class="tg-0pky">User Stories</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Enter the platform</td>
    <td class="tg-0pky">Access to the platform</td>
    <td class="tg-0pky">As a developer, do I want to ensure that only university/school students/just NUS members can access the platform as a safety measure?</td>
  </tr>
  <tr>
    <td class="tg-c3ow" rowspan="4"><br><br>Join a study group<br><br><br></td>
    <td class="tg-0pky" rowspan="2">Browse study group based on interested subject<br><br></td>
    <td class="tg-0pky">As a developer, I want to provide users with a list of available study groups according to the module he/she inserts</td>
  </tr>
  <tr>
    <td class="tg-0pky">As a user, I want to know the list of existing study groups based on the module I input</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="2">Pick a study group based on preferred time slot<br><br></td>
    <td class="tg-0pky">As a developer, I want to enable users to know the timeslot of each available study group sessions</td>
  </tr>
  <tr>
    <td class="tg-0pky">As a user, I want to choose to join a study group based on the timeslot that suits me</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="4"><br>Create a study group<br><br></td>
    <td class="tg-0pky">Insert a module</td>
    <td class="tg-0pky">As a host, I want to create a new study group by first inserting my module</td>
  </tr>
  <tr>
    <td class="tg-0pky">Insert a time slot</td>
    <td class="tg-0pky">As a host, I want to insert my desired time slot</td>
  </tr>
  <tr>
    <td class="tg-0pky">Insert max no of participants</td>
    <td class="tg-0pky">As a host, I want to limit the number of participants for my study group sessions to avoid overcrowding</td>
  </tr>
  <tr>
    <td class="tg-0pky">Insert meeting details</td>
    <td class="tg-0pky">As a host, I want to able to key in my meeting details.</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="5"><br>Manage vacancy<br><br></td>
    <td class="tg-0pky" rowspan="5"><br>Handle number of participants in a study group<br><br></td>
    <td class="tg-0pky">As a developer, I want to make a study group available if it is still vacant</td>
  </tr>
  <tr>
    <td class="tg-0pky">As a developer, I want to make a study group no longer visible to user</td>
  </tr>
  <tr>
    <td class="tg-0pky">As a user I want to see the number of vacancies left and total number of participants in a study group (e.g. 5/8)</td>
  </tr>
  <tr>
    <td class="tg-0pky">As a user, I want to be able to control the number of participants I let into my study group.</td>
  </tr>
  <tr>
    <td class="tg-0pky">As a host, I might want to close all vacancies after a certain point of time.</td>
  </tr>
  
  <tr>
    <td class="tg-0pky">Chat</td>
    <td class="tg-0pky">Chat with other users</td>
    <td class="tg-0pky">As a user, I want to be able to chat with other users to liven up the study atmosphere.</td>
  </tr>
</tbody>
</table>

<h2> Technologies used </h2>
-Firebase <br>
-React Native <br>
-Redux <br>

<h2> How are we different from other similar platforms? </h2>

<h3>Build in group chat forums: </h3>
Questions can be asked and answered within the study groups, but the focus of the application is for the creation of said study groups and enabling people from a module to create such a study group in the first place.

<h3>Telegram/Other messaging applications: </h3>
We provide a messaging feature for easy communication between study group members, and for the sharing of notes. Unlike other messaging apps, you do not need to be invited to join a study group on this application. 

<h2> Our features </h2>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Feature </th>
    <th class="tg-0lax">Functionality</th>
  </tr>
</thead>
<tbody>
  <tr>
    <th class="tg-0lax" colspan="2"><span style="font-weight:bold">User Account Management</span></th>
  </tr>
  <tr>
    <td class="tg-0lax">Log-in</td>
    <td class="tg-pys6">Allows users to enter their credentials and sign-in to their account of the app if they had already created one.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Log-out</td>
    <td class="tg-ql4m">Allows the users to sign out of their app and brings them back to the log-in page.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Sign up</td>
    <td class="tg-pys6">Allows users to create a new account with their email-address. Upon signing up, the users need to verify their email address before signing in.</td>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2"><span style="font-weight:bold">Homepage</span></th>
  </tr>
  <tr>
    <td class="tg-0lax">Change profile pic</td>
    <td class="tg-0lax">Allow users to customize their profile picture.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Change cover pic</td>
    <td class="tg-0lax">Allow users to customize their cover picture.</td>
  </tr>
  <tr>
    <td class="tg-0lax">My group list</td>
    <td class="tg-0lax">Allow users to view the groups they have joined or created.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Join a group</td>
    <td class="tg-0lax">Allow users to join a study session they are interested in.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Create a group</td>
    <td class="tg-0lax">Allow users to create a study session with their preferred timeslot.</td>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2"><span style="font-weight:bold">My Group List</span></th>
  </tr>
  <tr>
    <td class="tg-0lax">View</td>
    <td class="tg-0lax">Allow users to view the group details such as meeting date and time, access to the meeting link.</td>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2"><span style="font-weight:bold">Chat</span></th>
  </tr>
  <tr>
    <td class="tg-0lax">Send message</td>
    <td class="tg-0lax">Allow users to interact with other users within the same session via chat function.</td>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2"><span style="font-weight:bold">Connect meeting apps</span></th>
  </tr>
  <tr>
    <td class="tg-0lax">Direct access to other meeting websites or apps</td>
    <td class="tg-0lax">Allow users to connect to other meeting apps such as Google Meeting or Zoom within the app.</td>
  </tr>
 
</tbody>
</table>

<h2> Our development plan </h2>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Milestone 1</th>
    <th class="tg-0lax">Milestone 2</th>
    <th class="tg-0lax">Milestone 3</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">1. Add login and signup features and have firebase as backend user management tool.</td>
    <td class="tg-0lax">1. Complete the create a study session feature.<br>2. Complete the join a study session feature.<br>3. Complete the view my group list feature.<br>4. Add additional features such as upload notes and chat to each groups.<br>5. Add customize features such as able to change profile picture.<br>6. Perform minimal system testing.</td>
    <td class="tg-0lax">1. Perform bulk user testing.<br>2. Fix bugs.<br>3. Complete the implementation of the upload notes feature and chat function.<br>4. Add additional features.</td>
  </tr>
</tbody>
</table>

<h2> Milestone 2 </h2>
<h3> Core features developed </h3>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Features</th>
    <th class="tg-0lax">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Create a study session</td>
    <td class="tg-0lax">Users can create a session by inputting their desired timeslot and subject, and also provide their meeting link. <br>The system will then check if the meeting details the user input is valid, if there is an error, it will prompt the user to key in again.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Join a study session</td>
    <td class="tg-0lax">Users can browse through a list of upcoming study sessions and can join if the user is interested. A study session will no longer be visible if it hits the maximum capacity set by the host, or it has passed the meeting date.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Direct access to zoom</td>
    <td class="tg-0lax">Users will not be required to remember the meeting details. Just click on the meeting link and they will be directed to the meeting.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Chat within a group</td>
    <td class="tg-0lax">Users can engage in informative chat sessions through our build-in chat feature.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Customization</td>
    <td class="tg-0lax">Users can further customize their profile picture and cover picture within the app.</td>
  </tr>
</tbody>
</table>
<h3> Additional features to be developed during Milestone 3 </h3>


<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Features</th>
    <th class="tg-0lax">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Filter</td>
    <td class="tg-0lax">Users can filter search the groups they want to join via searching for the subject in the search bar.</td>
  </tr>
  <tr>
    <td class="tg-0lax">Upload resources</td>
    <td class="tg-0lax">Users can share their resources to the group or download other users' shared notes to their device.</td>
  </tr>
</tbody>
</table>

<h3> Problems encountered & System testing </h3>
<h4> System testing 1 - Customization : Profile pic and cover pic </h4>
Problems encountered: <br>
1. The uri provided is the local file path of the user's device. It has no problem to render the picture when the user logs in to the device he uses to upload the image. However, when he changes to other devices and log in, the profile pic fails to render. <br>
2. Upon creating an account and using the app for the first time, the profile pic and cover pic is blank (the user hasn't choose their images) , so some users might not know they can customize their profile pic. [Problem solved by a default profile pic and cover pic will  show up before the user changed their profile pic and cover pic.] <br>

<h4> System testing 2 - Create a group function </h4>
Problems encountered: <br>
None . <br>
The create function works well, and the system will make sure the input details are correct before they allow the users to create a study session.<br>
However, how can the system detect when some users are abusing the system ? [Additional function that can add to Milestone 3: Maybe we can limit the groups a user can create?]

<h4> System testing 3 - Join a group function </h4>
Problems encountered: <br>
1. Upon clicking the join button, the user information will be updated to firebase, but the screen does not refresh automatically, and the group that the user just joined still show up on the screen. Only if the user exits the join screen and reenter the screen, the data will be updated. [Problem solved by everytime a user join the group, we direct them to our homepage and a pop up message will show that they have successfully join the group.] <br>
2. What if the user wants to remove himself from the group? or acidentally press the join button? [Additional function that can add to Milestone 3: Remove a member from the group]

<h4> System testing 4 - Chat function </h4>
Problems encoountered: <br>
1. Rendering chat avatar if use profile pic as chat avatar (same issue as mentioned in System testing 1) [Problem solved by rendering user initials as chat avatar]

<h4> System testing 5 - Direct to zoom meeting function </h4>
Problems encountered : <br>
None. Works fine.

<h2> Milestone 3 </h2>
<h3> Additional features developed </h3>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Features</th>
    <th class="tg-0pky">Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Filter search</td>
    <td class="tg-0pky">Users can filter search the groups they want to join via searching for the subject in the search bar.</td>
  </tr>
 
</tbody>
</table>

### User Testing
Here are the results:
[User Testing Questionnaire Summary](https://github.com/MelissaChengPeiYee/Orbital_StudyBuddy/blob/main/doc/UserTesting.md)


### External links 

- [User Guide](https://github.com/MelissaChengPeiYee/Orbital_StudyBuddy/blob/main/doc/UserGuide.md)
- [Developer Guide](https://github.com/MelissaChengPeiYee/Orbital_StudyBuddy/blob/main/doc/DeveloperGuide.md)
- [Project Log](https://github.com/MelissaChengPeiYee/Orbital_StudyBuddy/blob/main/doc/ProjectLog.md)
