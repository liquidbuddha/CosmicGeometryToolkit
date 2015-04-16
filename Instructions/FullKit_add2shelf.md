--------------------------------------------------------------------------------
Add liquidbuddha Drop-down Menu
--------------------------------------------------------------------------------

Mac: HD/Users/User_Account/Library/Preferences/Autodesk/maya/scripts
Windows: C:\Documents and Settings\User_Account\My Documents\maya\scripts

-Place the following files in your Maya scripts folder, shown above
	lbsToolMenuFull.mel 
	miniKit.mel
	lbs_Custom_Tools_UI_LOCAL.mel

-Place the following FOLDER in your Maya scripts folder, shown above
	lbsToolkit (which includes seven additional folders, Phi_Tap, Evolute_Tab, etc)


-If there is already a userSetup.mel file in the scripts folder, copy the two lines from the lbsToolkit userSetup.mel and add to the userSetup.mel in the scripts folder.

-If there is not a userSetup.mel file in the scripts folder, place the lbsTookit userSetup.mel into the scripts folder.

-Relaunch Maya


--------------------------------------------------------------------------------
Add toolkit to shelf
--------------------------------------------------------------------------------
Open Script Editor
	-Window->General Editors->Script Editor

Open miniKit.mel
	in Script Editor
	File->Load Script

Select All lines of script
Middle Mouse drag to shelf

Open Shelf Editor
	-Window->Settings/Preferences->Shelf Editor

There are three tabs at the top left of the window "Shelves" "Command" "Double Click Command"
	
	-Select "Shelves Tab"
	-On the left half there are a list of shelves. Select shelf to add the toolkit to.
	-In "Shelf Contents" on the right, select icon for "New Item".
	-"User Script" created - Select "User Script" and switch to "Command" tab
	-Replace text in field with miniKit.mel.
	-Close Shelf Editor
