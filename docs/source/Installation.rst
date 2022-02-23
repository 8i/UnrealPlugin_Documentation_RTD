============================================================
Installation
============================================================

Adding the Eighti Plugin to an existing project
--------------------------------------------
- Close the Unreal Editor
- If one does not already exist, create a new folder in your project and name it ``Plugins``
- Unzip the donwloaded package and copy the ``plugin\EightiPlugin`` folder to your ``Plugins`` folder. The final structure should look like:

::

    Plugins
        |
        ----EightiPlugin
            |
            ----Config
            ----Content
            ----Resources
            ----Source
            ----ThirdParty
            ----EightiPlugin.uplugin


- Launch the Unreal Editor and load your project
- Open the ``Plugins`` window from ``Edit/Plugins`` at the top of the Editor window.
- In the left panel, scroll down and click on the ``Project/Other`` category
- Ensure the ``EightiPlugin`` plugin is listed and is enabled

Setting up Visual Studio Solution
---------------------------------
- Right click on ``EightiPluginExample.uproject`` and select ``Generate Visual Studio project files``. If you have multiple version of Unreal Engine installed, make sure you also choose ``Switch Unreal Engine version...`` and select the currently supported Unreal Engine version.
- Open ``EightiPluginExample.sln``
- Set *Games/EightiPluginExample* as the startup project.
- Depending on if you need to debug into Unreal Engine code, you can choose build configuration as ``Debug Editor`` for complete debuggable Unreal Engine, game and plugin code; or choose ``Debug Game Editor`` for just debugging game and plugin code; or choose ``Development Editor`` as an reasonably optimised Unreal Engine, game and plugin code. Note if you want to debug into Unreal Engine code, you need to build Unreal Engine from source. See https://docs.unrealengine.com/en-US/Programming/Development/BuildingUnrealEngine/index.html
- Press F5 to build and run.

Debugging Packaged Builds
-------------------------
- Open the Unreal Editor
- Open the Project
- From the file menu select ``Package Project/Packaging Settings``
- Ensure that the ``Build Configuration`` is ``DebugGame``
- Ensure that ``Include Debug Files`` is ticked
- From the file menu select ``Package Project/Windows/Windows (64bit)``
- Select a folder and wait for the build to complete
- Once complete, launch ``EightiPluginExample.exe``
- Open ``EightiPluginExample.sln``
- Attach the Debugger to the ``EightiPluginExample`` process

Updating To A Newer Version
---------------------------
- Close the Unreal Editor.
- Delete the ``EightiPlugin`` folder from your project's ``Plugin`` folder
- Proceed with the steps above in ``Adding the EightiPlugin Plugin to an existing project``
