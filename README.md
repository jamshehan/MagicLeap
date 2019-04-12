# MagicLeap

Currently contains an empty new Unity project targeting LuminOS 0.20 for Magic Leap development. 

Followed these steps:

Launch the Unity Hub.

Specify your Project name, Location, and select 3D for Template, and then click Create Project.

unityhub.2019.1.newproject

The Unity Editor opens.

Install the Unity XR Legacy Input Helpers:

In the Unity Editor main menu, go to Window > Package Manager. The Packages dialog box opens.

From the Packages list, select XR Legacy Input Helpers. unity.xrlegacyinputhelpers

Click Install.

You may close the Packages dialog box.

Set the path to the Lumin SDK:

Go to Edit > Preferences (Windows) or Unity > Preferences (macOS). The Preferences dialog box opens.
In the Preferences dialog box, click External Tools.
Under External Tools, click Browse and then select the Lumin SDK folder. Typically, /Users/user/MagicLeap/mlsdk/v0.xx.0.
You may close the Preferences dialog box.
Switch the Build Settings platform to Lumin:

Go to File > Build Settings.
From the Platform list, select Lumin and then click Switch Platform.
You may close the Build Settings window.
Set the required Player settings for Lumin:

Go to Edit > Project Settings.
Select Player.
Click the unity.icon.luminsettings.red tab.
In Other Settings, change Color Space to Linear.
In XR Settings, select the Virtual Reality Supported check box.
In XR Settings, change Stereo Rendering Mode to Single Pass Instanced.
You can close Project Settings.
Import the Magic Leap Unity Package:

Go to Assets > Import Package, and then click Custom Package.
In the Import package dialog box, browse to the MagicLeap.unitypackage file you installed with Magic Leap Package Manager. It is typically located in Users/user/MagicLeap/tools/unity/v0.xx.0.
In the Import Unity Package dialog box, click All and then click Import.
Replace the Main Camera in your scene with the Magic Leap prefab Main Camera:

In the Hierarchy window, delete Main Camera from SampleScene.
Select the Project window, go to Assets > MagicLeap > Core Components, and then drag Main Camera to SampleScene in the Hierarchy window. unity.dragmaincameracomponent
Copy the manifest.xml from the Examples folder to your project's Assets folder:

In the Project window, go to Assets > MagicLeap > Examples > Plugins > Lumin.
Right-click manifest, and then click Show in Explorer (Windows) or Reveal in Finder (macOS).
Using Windows Explorer or macOS Finder, copy the manifest.xml file into your Unity project's Assets/Plugins/Lumin folder—if this folder does not exist, create it.
You are now ready to develop Magic Leap apps in Unity.

