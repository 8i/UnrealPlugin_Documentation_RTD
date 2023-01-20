============================================================
PATActor
============================================================

``PAtActor`` is the main object you will be interacting with from the 8i Unreal Plugin.

How To Create
=============

1. From ``Place Actor`` window, search ``PATActor``, or you can scroll down from the ``All Classes`` list, then drag and drop an ``PATActor`` to your scene.
2. In the Details Panel, expand the ``Eighti`` options, use Content Browser, or browsing from the dropdown list to assign an ``PATAsset`` asset to the ``PATActor``.

Parameters
==========

Audio
-----
**Attentuation Parameters**
    Modify this object to correctly model the 3D sound emanating from the PATActor

Eighti
------

**PAT Data Asset**
    This links the PATActor to the PATAsset it should load during play.    
	
**Playing Status**
	This enum is queryable from blueprints and gives the status of whether or not the asset is currently playing.
	
**Open Status**
	This enum is queryable from blueprints and gives the status of whether or not the asset is currently opened.

[Details] Init Controls
-----------------------

These values are only settable when the asset is not currently open. They control instance wide aspects of the asset.

**Enable Logging**
    Should a log be created.

**Use Verbosity**
    Should verbose output be used in the log if created.

**Loop Playback**
    Should playback be looped after finished?
	
**Playback Speed**
    This sets the playback speed to be faster or slower depending on the multiplier chosen.
	
[Details] Playback Info
-----------------------

These values are only set during playback when an asset is running and give some metadata information about the asset.

**Asset Frame Rate**
The current framerate of the asset.

**Asset Duration**
The duration of the asset in seconds.

**Current Frame timestmap**
The timestamp of the frame currently being rendered.

[Details] Playback Controls
---------------------------

These values can be used to help trim an asset in case a shorter duration is required than the entire take.

**Start Time**
If non-zero, the start time of the asset in seconds.

**End Time**
If non-zero, the end time of the asset in seconds.
	
[Details] Material
------------------

These values can be used to help control the appearance of the rendered asset.

**Render Mode**
    Unlit -> the actor will be treated as an unlit material.
	Lit -> The actor will be treated as a lit material.

**Emissive Strength**
    Modifier to the relative color brightness in the Unlit Render Mode. Values range from 0 to 10.0

**Specular**
    Modifier that adjusts light reflectivity. Values range from 0.0 to 1.0
	
**Roughness**
    Modifer that adjusts light scattering. Values range from 0.0 to 1.0