============================================================
Quick Start
============================================================

Create a scene
------------------------------------------------------------

1. Install the HVR plugin ( see Installation for steps ) to your existing project
2. Make a folder in Content Browser under ``Content``, naming could be arbitrary.
3. Drag and drop any .8i or .hvrs file on your local drive to that folder. This should import the .8i/.hvrs file reference and create an Unreal asset of type ``UHVRLinkAsset`` in that folder.
4. Make sure the original .8i/.hvrs file exists in the same place while your project is in development, otherwise the asset needs to be modified or re-imported.
5. From ``Place Actor`` window, search ``HVRActor``, or you can scroll down from the ``All Classes`` list, then drag and drop an ``HVRActor`` to your scene.
6. Select the ``HVRActor`` by clicking the pink 8i logo on it.
7. Navigate to the imported asset in Content Browser, keep it selected.
8. Optionally, press Ctrl-S to save the asset.
9. In the Details Panel, expand the ``HVRActor`` options, click the small '<-' button next to the thumbnail. It will assign the asset to the ``HVRActor``.
10. A 8i HVR hologram should be shown in the viewport.

Create a build
------------------------------------------------------------

When packaging a build, there is one thing to notice is 8i's content needs a special ``cooking`` process. Normally the cooking happens after you save the UHVRLinkAsset object in Content Browser. But if anything went wrong, you can always do the cooking process manually, before packaging a build:

1. Click the 8i logo on the main toolbar, next to the 'Settings' button.
2. Choose ``Rebuild 8i Contents``. This will search all the imported 8i assets(of type UHVRLinkAsset) and copied them into a folder called ``8iCooked``.
3. Check the ``Window / Developer Tools / Output Log`` to see if anything wrong. Normally you will see a message says ``LogHVRPlayerEditor: Re-cooked all 8i contents``.

The rest of the build process remains the same for your project.
