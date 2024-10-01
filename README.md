> Why do I have a folder named ".expo" in my project?
The ".expo" folder is created when an Expo project is started using "expo start" command.
> What do the files contain?
- "devices.json": contains information about devices that have recently opened this project. This is used to populate the "Development sessions" list in your development builds.
- "settings.json": contains the server configuration that is used to serve the application manifest.
> Should I commit the ".expo" folder?
No, you should not share the ".expo" folder. It does not contain any information that is relevant for other developers working on the project, it is specific to your machine.
Upon project creation, the ".expo" folder is already added to your ".gitignore" file.


my report 
I began my journey by creating a new React Native project named MastPOE using the command:npx react-native init MastPOE
During the initialization process, i received a warning about the deprecation of the init command, which suggested that i  should switch to using:npx @react-native-community/cli init
After successfully creating the project, I  encountered issues when trying to run my  application on Android. i  ran the command:npx react-native run-android
However, the process failed with an error indicating that the Android project could not be found. This prompted me to reinitialize the project correctly. After resolving the structure, i proceeded to install the necessary packages for navigation within my app. I installed the core React Navigation package:npm install @react-navigation/native
Additionally, i installed the stack navigation package:npm install @react-navigation/stack
To ensure that my app could handle gestures and manage screens properly, i installed several other dependencies:npm install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view
With my navigation packages installed, i moved on to writing the code for my application. In the App.tsx file, i  set up a basic navigation structure. i  created a stack navigator that includes several screens such as Home, Courses, Starters, Main, Desert, Available Now, and Chef Description. i  used the NavigationContainer to wrap my  navigator and set the initial route.

However, when i tried to run the application again, i faced multiple issues. The first issue was a conflict with port 8081, which was already in use by another process, prompting me  to switch to port 8082. Following that, i  encountered an error indicating that the ADB (Android Debug Bridge) command was not recognized on my system, suggesting a potential issue with my  Android SDK setup.

Additionally, i  received an error indicating that no Android emulators were found. This was likely due to a lack of properly configured virtual devices or an emulator setup. The final blow came when the build failed due to an issue in the settings.gradle file, indicating a missing plugin and problems with file access.

To resolve these issues, i  ran the command:npm install
This completed without any vulnerabilities but did produce warnings about several deprecated packages, suggesting that some of the packages i were using were no longer maintaine
Overall, i  made significant progress in setting up my  React Native application and began implementing navigation. However, i encountered several technical hurdles, particularly related to the Android environment, that prevented me from successfully launching my application. Suggestions for resolving these issues include checking my emulator setup, ensuring ADB is correctly recognized, and using GestureHandlerRootView for wrapping my application if necessary.

