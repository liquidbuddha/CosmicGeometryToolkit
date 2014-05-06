CosmicGeometryToolkit by liquidbuddha (R)
=========================================

visual effects toolkit for Autodesk Maya, enabling fast creation of toroidal evolutionary wavefronts, flower of life patters, jitterbugging vector equlibrium, geometric primatives, and more.  Two toolkits are available in two flavors, the minikit and full-kit.

miniKit
=======
miniKit: this version includes the following functionality
 - customizable torus evolute tool
 - customizable phi-spiral & vortex creation tool
 - customizable bonus Rodin-like Evolute tool

Full Toolkit
============
Full-Kit includes Seven (7) tabs, each with expanded functionality related to the tab's theme. The function-tabs include:

Evolute Tab:
 - custom toroidal evolute path creation 
 - multi-evolute management and editing
 - "tapered bead" option, which auto-animates a series of tapered spheres, along the evolute path. an amazing toroidal simulation tool

Radiating Tab:
 - automated creation of evolute path extrudes in series
 - editable in instance scale
 - auto coloration option
 - multi array management and editing

Phi-Tab
 - creation of phi curve, or vortex
 - multi-vortex management and editing
 - phi-conn option .. connects two 3D phi-vortex arrays
 - connect to Jitterbug option ... connects to Jitterbugging VE models in VE tab

FOL Tab (Flower of Life)
 - create a flower of life matrix of curves or extrudes to "n" layers
 - automate it's replication in 2D, 3D, 4D, or 6D geometries
 - multi FOL array management and editing

Jitterbug Tab
 - create a jitterbugging VE or VE matrix (jitterbug is the VE breathing from compressed states, matrix unifies the triangular faces to form interconnected counter-breathing chains of jitterbugging VEs
 - multi VE matrix management and editing

Geo Tab (Geometry)
 - instant creation of any platonic solid, with option to extrude
 - scale control
 - multi-geometry management and editing
 - shapes include: tetrahedron, tetrahedron dual, Cube, Octahedron, Icosohedron, Dodecahedron, Vector EQ, and finally the Rhombic-dodecahedron.
 - all geometries are created in perfect alignment with Metatron's Cube configuration, where all geometries and symmetries are unified

Star Tab
 - automated transformation of "space brush" brush-strokes into polygons or image planes, which adds greater control for rendering of space-brush star-fields.


==============================

Install Instuctions:

1) Download and unzip the Full Install archive.

2) Place the following files in your Maya scripts folder, shown above
      	lbsToolMenuFull.mel 
      	miniKit.mel
      	lbs_Custom_Tools_UI_LOCAL.mel

  for Mac users, the Maya scripts folder is:    HD/Users/User_Account/Library/Preferences/Autodesk/maya/scripts
  for Windows users:                            C:\Documents and Settings\User_Account\My Documents\maya\scripts

3) Place the following FOLDER in your Maya scripts folder, shown above
      	lbsToolkit (which includes seven additional folders, Phi_Tap, Evolute_Tab, etc)


4) If there is already a userSetup.mel file in the scripts folder, copy the two lines from the lbsToolkit userSetup.mel and add to the userSetup.mel in the scripts folder.

5) If there is not a userSetup.mel file in the scripts folder, place the lbsTookit userSetup.mel into the scripts folder.

6) Relaunch Maya

Additional instructions for miniKit installations, and adding the toolkit to the Maya shelf, are included in the "Instructions" folder.
