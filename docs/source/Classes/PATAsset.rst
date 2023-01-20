============================================================
PATAsset
============================================================

Used to help simplify loading of the native data behind a PATActor

How To Create
------------------------------------------------------------
There are two methods to create a Pat actor.

If you are primarly using hosted content then the normal flow will be to:
1. Create a new ``PATAsset`` content object.
2. In the Details panel, fill in the Remote URI with the appropriate manifest file. (ex: http://my/hosted/content/path/manifest.mpd)
3. Set the ``PAtAsset`` Source dropdown to be Remote
4. If you wish to download this remote data, right click on the asset and click Download(). Then set the Source field to be 'Local'

If you are primarly using predownloaded content then the normal flow will be to:
1. Drag and Drop a pre-existing .8iPat file into the Content Browser. An asset will automatically be created with the appropriate fields set up.
2. The `Remote Uri` field will not be set in this case and should remain unpopulated.
3. The `Source` field should be set to `Local` 

Parameters
------------------------------------------------------------

**Remote URI**
    This should hold the path to the remote manifest file (ex: http://my/hosted/content/path/manifest.mpd)

**Local URI**
    After Downloading completes, this should hold the path to the local manifest file (ex: $(ProjectDir)/content/high/eighti/<name>/manifest.txt)

**Source**
    Drop down menu to select either Remote or Local Data for this asset to reference.

Actions
-------

**Download()**
    Downloads the content indicated in the Remote URI to the project local content directory. This will autopopulate the Local URI parameter.
	
**Generate Preview Frame()**
	This created a local preview of the asset within the editor to aid with placement and lighting. 
