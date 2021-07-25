# **Orbital 2021 System Testing** 

## Team Study Buddy 

* [**Orbital 2021 System Testing** ](#orbital-2021-system-testing)
    * [Team Study Buddy](#team-study-buddy) 
        * [System testing by screens](#system-testing)
            
           
### System Testing

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Categorized by screen</th>
    <th class="tg-0pky">Features</th>
    <th class="tg-0pky">What it does</th>
    <th class="tg-0pky">Pass/Fail</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky" rowspan="2">First-time user screen (src/screens/Main)</td>
    <td class="tg-0pky">Create an account button</td>
    <td class="tg-0pky">Navigate to sign up screen </td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">"Log in here" text in red</td>
    <td class="tg-0pky">Navigate to login screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="3">Sign up screen (src/screens/Signup)</td>
    <td class="tg-0pky">Eye icon at password column</td>
    <td class="tg-0pky">Make password visible or invisible</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Sign Up button</td>
    <td class="tg-0pky">Allow users to sign up, send verification email and navigate to Login screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">"Log in here" text in red</td>
    <td class="tg-0pky">Navigate to login screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="3">Login screen (src/screens/Login)</td>
    <td class="tg-0pky">Eye icon at password column</td>
    <td class="tg-0pky">Make password visible or invisible</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Sign In button</td>
    <td class="tg-0pky">Allow users to login, and navigate to Home screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">"Create one here" text in red</td>
    <td class="tg-0pky">Navigate to sign up screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="7">Home screen (src/screens/Home)</td>
    <td class="tg-0pky">"Change cover photo?" text in blue</td>
    <td class="tg-0pky">Allow users to change cover photo, navigate to Coverpic screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Round profile pic button</td>
    <td class="tg-0pky">Allow users to change profile photo, navigate to Profilepic screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Username</td>
    <td class="tg-0lax">Whether the username is correct</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">YOUR GROUP LIST button</td>
    <td class="tg-0pky">Allow users to view their group lists, navigate to Dashboard screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">JOIN A STUDY GROUP button</td>
    <td class="tg-0pky">Allow users to join study groups, navigate to Join screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">CREATE A STUDY GROUP button</td>
    <td class="tg-0pky">Allow users to create study groups, navigate to Precreate screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">"Sign out" text in red</td>
    <td class="tg-0pky">Allow users to sign out, navigate back to Login screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="2">Profilepic screen (src/screens/Profilepic)</td>
    <td class="tg-0pky">"PICK A PROFILE PIC" text in purple</td>
    <td class="tg-0pky">Upon clicking, able to choose images from device</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">"SET AS PROFILE PIC" text in purple</td>
    <td class="tg-0pky">Upon clicking, navigate to Home screen, and profile pic changed to new one</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="2">Coverpic screen (src/screens/Coverpic)</td>
    <td class="tg-0pky">"PICK A COVER PIC" text in purple</td>
    <td class="tg-0pky">Upon clicking, able to choose images from device</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">"SET AS COVER PIC" text in purple</td>
    <td class="tg-0pky">Upon clicking, navigate to Home screen, and cover pic changed to new one</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="2">Precreate screen (src/screens/Precreate)</td>
    <td class="tg-0pky">Back button in blue</td>
    <td class="tg-0pky">Navigate to Home</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Proceed to Create button</td>
    <td class="tg-0pky">Navigate to Create screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax" rowspan="9">Create screen (src/screens/Create)<br><br><br><br><br><br><br></td>
    <td class="tg-0lax">Back button in blue</td>
    <td class="tg-0lax">Navigate to Precreate screen</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Insert module text input</td>
    <td class="tg-0pky">Able to key in module</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Start time picker</td>
    <td class="tg-0pky">Able to pick start time</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">End time picker</td>
    <td class="tg-0pky">Able to pick end time</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Participants drop down picker</td>
    <td class="tg-0pky">Able to pick no of participants</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Insert zoom link text input</td>
    <td class="tg-0pky">Able to key in zoom link</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Insert zoom code text input</td>
    <td class="tg-0pky">Able to key in zoom code</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">Insert zoom password text input</td>
    <td class="tg-0pky">Able to key in zoom password</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky">CREATE STUDY GROUP button</td>
    <td class="tg-0pky">Send data to Firestore, check valid time and date, navigate to Postcreate screen</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="2">Postcreate screen (src/screens/Postcreate)</td>
    <td class="tg-0pky">Study group details</td>
    <td class="tg-0pky">Whether the details matches with the one just keyed-in</td>
    <td class="tg-0pky">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">BACK TO HOME SCREEN button</td>
    <td class="tg-0lax">Navigate to Home screen</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax" rowspan="4">Join screen (src/screens/Join)</td>
    <td class="tg-0lax">Search bar</td>
    <td class="tg-0lax">Whether search function works</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Displaying group lists</td>
    <td class="tg-0lax">Whether the correct group lists are displayed (except the ones the user created or have joined)</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Join icon button</td>
    <td class="tg-0lax">Allow users to join group, a confirmation pops out, navigate back to Home screen</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Back button on device</td>
    <td class="tg-0lax">Navigate back to Home screen</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax" rowspan="3">Dashboard screen (src/screens/Dashboard)</td>
    <td class="tg-0lax">Displaying group lists</td>
    <td class="tg-0lax">Whether the correct group lists are displayed and in chronological order (the ones the user created or have joined)</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">View icon button</td>
    <td class="tg-0lax">Allow users to view group info, navigate to Tab screen</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Back button on device</td>
    <td class="tg-0lax">Navigate back to Home screen</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax" rowspan="3">Details screen (src/screens/Details)</td>
    <td class="tg-0lax">Zoom meeting details</td>
    <td class="tg-0lax">Whether the information is correct</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Zoom link</td>
    <td class="tg-0lax">Upon clicking, direct to the website</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Back button on device</td>
    <td class="tg-0lax">Navigate back to Home screen</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax" rowspan="4">Chat screen (src/screens/Chat)</td>
    <td class="tg-0lax" rowspan="3">Chat </td>
    <td class="tg-0lax">Able to send messages </td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">View other users' messages</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Load previous messages</td>
    <td class="tg-0lax">Pass</td>
  </tr>
  <tr>
    <td class="tg-0lax">Back button on device</td>
    <td class="tg-0lax">Navigate to first tab</td>
    <td class="tg-0lax">Pass</td>
  </tr>
</tbody>
</table>
