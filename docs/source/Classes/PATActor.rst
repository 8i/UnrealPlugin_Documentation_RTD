============================================================
PATActor
============================================================

``PAtActor`` is the main object you will be interacting with from the 8i Unreal Plugin.

A ``PATActor`` can specify a data URI and be used to render PAT content.

How To Create
-------------

1. From ``Place Actor`` window, search ``PATActor``, or you can scroll down from the ``All Classes`` list, then drag and drop an ``PATActor`` to your scene.
2. In the Details Panel, expand the ``PATActor`` options, use Content Browser, or browsing from the dropdown list to assign an ``PATAsset`` asset to the ``PATActor``.

Parameters
----------

## Audio 

**Attentuation Parameters**
    Modify this object to correctly model the 3D sound emanating from the PATActor
	
## EightI	

**PAT Data Asset**
    This links the PATActor to the PATAsset it should load during play.    

**Enable Logging**
    Should a log be created.

**Use Verbosity**
    Should verbose output be used in the log if created.

**Loop Playback**
    Should playback be looped after finished?

## Material

**Render Mode**
    Unlit -> the actor will be treated as an unlit material.
	Lit -> The actor will be treated as a lit material.

**Emissive Strength**
    Modifier to the relative color brightness in the Unlit Render Mode. Values range from 0 to 10.0

**Specular**
    Modifier that adjusts light reflectivity. Values range from 0.0 to 1.0
	
**Roughness**
    Modifer that adjusts light scattering. Values range from 0.0 to 1.0