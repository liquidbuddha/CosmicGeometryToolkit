Cosmic Geometry Toolkit by liquidbuddha.studios
===============================================

Visual effects toolkit for Autodesk Maya, enabling fast creation of toroidal evolutionary wavefronts, phi-spirals, flower of life patters, jitterbugging vector equlibrium, geometric primatives, and more.  The toolkit is available in two flavors, the full-kit and the minikit.

Examples, tutorials and other tips availabe at http://www.liquidbuddha.com/project-cosmic-geometry-toolkit/

Full Toolkit
============
Full-Kit includes Seven (7) tabs, each with expanded functionality related to the tab's theme. The function-tabs include:

Evolute Tab: [http://www.liquidbuddha.com/project-cosmic-geometry-toolkit/evolute-tab-creating-an-animated-toroidal-evolutionary-wavefront/]
 - custom toroidal evolute path creation 
 - multi-evolute management and editing
 - "tapered bead" option, which auto-animates a series of tapered spheres, along the evolute path. an amazing toroidal simulation tool

Radiating Tab: [http://www.liquidbuddha.com/project-cosmic-geometry-toolkit/radiating-tab-creating-stacked-evolutionary-radiating-systems/]
 - automated creation of evolute path extrudes in series
 - editable in instance scale
 - auto coloration option
 - multi array management and editing

Phi-Tab: [http://www.liquidbuddha.com/project-cosmic-geometry-toolkit/phi-tab-creating-animated-phi-spiral-vortex-systems/]
 - creation of phi curve, or vortex
 - multi-vortex management and editing
 - phi-conn option .. connects two 3D phi-vortex arrays
 - connect to Jitterbug option ... connects to Jitterbugging VE models in VE tab

FOL Tab (Flower of Life) : [http://www.liquidbuddha.com/project-cosmic-geometry-toolkit/fol-tab-creating-flower-of-life-patterns-in-multi-dimentions/]
 - create a flower of life matrix of curves or extrudes to "n" layers
 - automate it's replication in 2D, 3D, 4D, or 6D geometries
 - multi FOL array management and editing

Vector Equilibrium [Jitterbug] Tab: [http://www.liquidbuddha.com/project-cosmic-geometry-toolkit/vector-equilbrium-tab/ ]
 - create a jitterbugging VE or VE matrix (jitterbug is the VE breathing from compressed states, matrix unifies the triangular faces to form interconnected counter-breathing chains of jitterbugging VEs
 - multi VE matrix management and editing

Geo Tab (Geometry):[http://www.liquidbuddha.com/project-cosmic-geometry-toolkit/geometry-tab-c…-relationships/] 
 - instant creation of any platonic solid, with option to extrude
 - scale control
 - multi-geometry management and editing
 - shapes include: tetrahedron, tetrahedron dual, Cube, Octahedron, Icosohedron, Dodecahedron, Vector EQ, and finally the Rhombic-dodecahedron.
 - all geometries are created in perfect alignment with Metatron's Cube configuration, where all geometries and symmetries are unified

Star Tab: [http://www.liquidbuddha.com/project-cosmic-geometry-toolkit/star-replace-tab/]
 - automated transformation of "space brush" brush-strokes into polygons or image planes, which adds greater control for rendering of space-brush star-fields.

miniKit
=======
miniKit: this version includes the following functionality
 - customizable torus evolute tool
 - customizable phi-spiral & vortex creation tool
 - customizable bonus Rodin-like Evolute tool



Install Instructions
===================
1) Download and unzip the github archive.

2) Place the following three (3) files in your Maya scripts folder, depending on the folder location for your platform, shown below
-	lbsToolMenuFull.mel

- miniKit.mel

- lbs_Custom_Tools_UI_LOCAL.mel

  For Mac users, the Maya scripts folder is:    HD/Users/User_Account/Library/Preferences/Autodesk/maya/scripts

  For Windows users:                            C:\Documents and Settings\User_Account\My Documents\maya\scripts

3) Using a text editor, modify the following two lines from the lbsToolMenuFull.mel & miniKit.mel files, replacing "User_Account" with the path appropriate for your file system.

For Mac users, it's a simple name change.  For Windows users, you may need to add "C:\" and adjust the "/" to "\". 

	  menuItem -p $MyMenuObj -l "mini kit" -c ("source \"/Users/User_Account/Library/Preferences/Autodesk/maya/scripts/lbsToolkit/toolkit_dropDown/miniKit.mel\"; ");
	  menuItem -p $MyMenuObj -l "full kit" -c ("source \"/Users/User_Account/Library/Preferences/Autodesk/maya/scripts/lbsToolkit/lbs_Custom_Tools_UI_LOCAL.mel\"; ");

4) Finally, in the lbs_Custom_Tools_UI_LOCAL.mel file, make the same adjustments specific to your file system..

	string $scriptLoc = "/Users/User_Account/Library/Preferences/Autodesk/maya/scripts";

5) CREATE A NEW FOLDER in your Maya scripts folder (location shown above), and rename it...
- lbsToolkit

Place the following seven (7) folders into the lbsTookit folder...
- Evolute_Tab
- Phi_Tab
- FlowerOfLife_Tab
- RadiatingTori_Tab
- Jitterbug_Tab
- Geometry_Tab
- StarReplace_Tab

6) If there is already a userSetup.mel file in the scripts folder, copy the two lines from the lbsToolkit userSetup.mel and add to the userSetup.mel in the scripts folder.

7) If there is not a userSetup.mel file in the scripts folder, place the lbsTookit userSetup.mel into the scripts folder.

8) Relaunch Maya

--------------
If you are not using Maya2011, you will need to adjust line 208, in the "StarReplaceToolkit.mel" to reflect your version of Maya, and the path tho the Brushes.

	source "/Applications/Autodesk/maya2011/Maya.app/Contents/brushes/galactic/space.mel";
--------------

More Info:
==========
*Additional instructions for miniKit installations, and adding the toolkit to the Maya shelf, are included in the "Instructions" folder.

When the MEL code is loaded in Maya, you can also create many things from the command line. The evolute command is:

evoCurve (float $tRad, float $HR, int $NumLoops, float $CentRot, float $speed)
- $tRad is the Torus Radius
- $HR is the Height Ratio of the Torus. HR of 1 is a horn torus. .5 is a typical donut, .1 looks like a bicycle tire
- $NumLooks is the number of "loops" around the torus surface. One loop traverses the radial plane, and axial plan once.
- $CentRot is the center rotation between each step. Useful rance is 10-30 degres. Less than 10 creates a lot of overhead geometry, but may be useful for some. Also, over-rotating (using a CentRot of over 60 degrees yields some very interesting anomolies!
- $speed is the number of frames for a full evolutionary cycle

evoCurve (10, 1, 6, 15, 100);	    // a six loop horn torus evolute curve, with a radius of 10

Also, be sure to explore the Evolute_Tab's "Evolterate.mel" code, with which you can create multiple evolute curves, with itterative parameters.
