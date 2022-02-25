============================================================
PATActor
============================================================

``PAtActor`` is the main object you will be interacting with from the 8i Unreal Plugin.

A ``PATActor`` can specify a data URI and be used to render HVR content.

How To Create
-------------

1. From ``Place Actor`` window, search ``PATActor``, or you can scroll down from the ``All Classes`` list, then drag and drop an ``PATActor`` to your scene.
2. In the Details Panel, expand the ``PATActor`` options, use Content Browser, or browsing from the dropdown list to assign an ``PATAsset`` asset to the ``PATActor``.

Parameters
----------

**Attentuation Parameters**
    Modify this object to correctly model the 3D sound emanating from the PATActor

**PAT Data Asset**
    This links the PATActor to the PATAsset it should load during play.    

**Enable Logging**
    Should this HVR begin playing as soon as it is created?

**Use Verbosity**
    Should this HVR loop?

**Loop Playback**
    - FastCubes [Default]
        - The recommended way for rendering content. Renders each voxel in an adjacent cube style and avoid holes.
    - Point Sprite
        - Renders the actor with hard edges.
        - Renders faster than PointBlend

Actions
-------

**Open()**
    Blueprint function to prepare the native library to fetch, decode, and render the remote or local data linked in the PATAsset. This must be called before Play() or Pause()

**Close()**
    Closes out native libraries created in Open()

**Play()**
    Starts playback of the PatActor.

**Pause()**
    Pauses playback of the PatActor
