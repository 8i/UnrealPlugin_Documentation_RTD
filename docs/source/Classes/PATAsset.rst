============================================================
PATAsset
============================================================

Used to help simplify loading of the native data behind a PATActor

How To Create
------------------------------------------------------------

1. Create a new ``PATAsset`` content object.
2. In the Details panel, fill in the Remote URI with the appropriate manifest file. (ex: http://my/hosted/content/path/manifest.mpd)
3. Set the ``PAtAsset`` Source dropdown to be Remote

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
