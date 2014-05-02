Blender-Fulldome-Addon
======================

Download and install Hugin (http://hugin.sourceforge.net/download/).

Download DomeCam. To install the Blender addon, move the domecam.py into your scripts/addons folder.

Activate DomeCam inside of Blender.  Just as any other addon: User Preferences -> Addons -> Install Addon

Once installed and activated, there will be a new panel in the render tab.




nona is a part of the hugin installation and can be found in the HuginTools folder. Point the configuration "path to nona" to the executable.  If Blender can find the nona executable, it will stitch the images automatically -- there is no need for you to open Hugin.  This must be a direct path to nona.exe; a relative path will not render the image and produce error messages.

Edit your desired render-resolution (please use typical domemaster sizes like 512, 1024, 2048, 4096 etc).



You also have to setup your renderpath and filename in this panel (settings in the default blender panels will be overwritten once you start to render).

It is possible to run postprocessing on the finished domemaster. If you want to do this, enable the checkbox. Click the “Add Nodes for Domemaster processing” button, which will then add some nodes that will put a black border around the stitched image. You will need to render once after adding these nodes to see any changes to the domemaster.

Before you render, open up the system console.  (Help -> System Console)  This will enable you to view progress of the render.

To render, simply press the image button to render a single frame, or the animation button, to render the whole animation.  Ensure that you are using the render button inside of the DomeCam panel.

While blender is rendering, it won't give any feedback and won't react on any user input.  Blender has not crashed.  To get some feedback of what's going on look at the system console which will display messages after each camera render and domemaster stitching.
