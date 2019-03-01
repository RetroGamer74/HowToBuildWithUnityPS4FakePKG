# How To Build With Unity PS4 FakePKG
In order to build with success using Unity PS4 you need to be sure your setup is complete.

Setup
=====

1.- Install PS4 S*D*K. There is a release out there you have to look for. ( Krome Mods )

2.- Install Unity 2017.2.0p2. ( You have to look for the version capable to build for 4.55 PS4 release ).

3.- Install Unity PS4 2017.2.0p2 for the same release than Unity 2017 release.

4.- You can also install Monodevelop from the preferences menu option within Unity Editor. You can, anyway, install Visual Studio as IDE.

5.- Once PS4 S*D*K is installed you have to replace the Publishing Tools which are located in PATH_SDK/ORBIS/Tools/Publishing Tools/ with the FakePKG tools you can download from: https://mega.nz/#!aRgCzJDI!XyCqSXLAyO4wpsqkVb3Lhx8YxrZLGMPC9ARt8CxmEys

6.- Create a Unity account if you still don't have one.

7.- Set the license. You can do this in first Unity startup, or in the Help menu, by selecting Manage License. Then, select Activate License, and set yours.


Building
========

1.- Create a new project, or open an existing one, or just import one of the packages as samples you can also find out there.

2.- When you ready to build the project select File -> Build Settings.

3.- Set the window as show in next image.


![PC Hosted](https://github.com/RetroGamer74/HowToBuildWithUnityPS4FakePKG/blob/master/Captura1.PNG "Set PC Hosted")

4.- Now click in Player Settings button on the bottom left side of the Build Settings window.

![Other Settings](https://github.com/RetroGamer74/HowToBuildWithUnityPS4FakePKG/blob/master/Captura3.PNG "Other Settings")

5.- Usually the environment variables of the S*D*K are set in the system, and Unity does not require you set the S*D*K path, but I prefer to set it.

6.- Now press build Button. Take in mind, this build won't work. We do this build to retrieve 3 files we need for the final build. So in the File Dialog, create a new folder out of the project and set it a name. For example Build. And then select the folder and continue.

![Open Dialog](https://github.com/RetroGamer74/HowToBuildWithUnityPS4FakePKG/blob/master/Captura5.PNG "Open Dialog")

7.- When the built is complete browse the folder Build or the name you set and go to the sce_sys folder.

![Build Folder](https://github.com/RetroGamer74/HowToBuildWithUnityPS4FakePKG/blob/master/Captura6.PNG "Build Folder")

8.- Copy next 3 files from sce_sys folder.

![Build Folder](https://github.com/RetroGamer74/HowToBuildWithUnityPS4FakePKG/blob/master/Captura7.PNG "Build Folder")

9.- Paste the 3 files copied into the upper project folder

![Build Folder](https://github.com/RetroGamer74/HowToBuildWithUnityPS4FakePKG/blob/master/Captura8.PNG "Build Folder")

10.- We'll use those 3 files in the Publishing Settings of the Player Settings. So go back again to the Build Settings window. Press Player Settings button, and in the Inspector select the Publishing Settings. Now you have to use those 3 files in the options: Share parameter file to set shareparam.json, pronunciation.xml set to pronunciation.xml, and pronunciation.sig to pronunciation.sig. We have to do this because we're going to build a non development package, and to use that we have to set those 3 files.

![Publishing Settings](https://github.com/RetroGamer74/HowToBuildWithUnityPS4FakePKG/blob/master/Captura2.PNG "Publishing Settings")

11.- Finally set Build Settings -> Build Type: PS4 Package and remove any check from the checkboxes.

![Build Settings](https://github.com/RetroGamer74/HowToBuildWithUnityPS4FakePKG/blob/master/Captura.PNG "Build Settings")

12.- Set parental control to 1 in Publishing Settings. If you keep in value 11 which is default you will get an error about invalid parental control number.

13.- Now you can click Build, and you can do more builds without repeating all the steps shown here. You have to do this only once for the project. Remember you empty the folder Build before you try to compile again, because Unity requires build folder be empty if you are going to create a different Build Type, which is the case. We changed Build Type from PC Hosted to PS4 Package. After that you can build more times without clean folder while you create always PS4 Packages.


![License](https://img.shields.io/badge/License-GPLv2-blue.svg)
[![Chat on Discord](https://camo.githubusercontent.com/b4175720ede4f2621aa066ffbabb70ae30044679/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636861742d446973636f72642d627269676874677265656e2e737667)](https://discordapp.com/invite/cUnjkPH)
