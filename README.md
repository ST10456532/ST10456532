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
