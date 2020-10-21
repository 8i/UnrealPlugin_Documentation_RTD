============================================================
HVRActor
============================================================

``HVRActor`` is the main object you will be interacting with from the 8i Unreal Plugin.

A ``HVRActor`` can specify a data URI and be used to render HVR content.

How To Create
-------------

1. From ``Place Actor`` window, search ``HVRActor``, or you can scroll down from the ``All Classes`` list, then drag and drop an ``HVRActor`` to your scene.
2. In the Details Panel, expand the ``HVRActor`` options, use Content Browser, or browsing from the dropdown list to assign an ``HVRLinkAsset`` asset to the ``HVRActor``.

Parameters
----------

**Data Asset**
    Represents the actual .8i/.hvrs file that gets imported.

**Play on Awake**
    Should this HVR begin playing as soon as it is created?

**Loop**
    Should this HVR loop?

**Render Method**
    - FastCubes [Default]
        - The recommended way for rendering content. Renders each voxel in an adjacent cube style and avoid holes.
    - Point Sprite
        - Renders the actor with hard edges.
        - Renders faster than PointBlend
