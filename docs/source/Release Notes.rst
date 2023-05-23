==================================
Release Notes
==================================

v0.6.1
- [FEATURE ENHANCEMENT] : Added direct gpu<->gpu texture transfer path for hardware accelerated decode. This mode requires the renderer to be D3D11 capable.
- [FEATURE ENHANCEMENT] : Added a toggle to enable/disable audio.
- [BUGFIX] : Set the default project AA algorithm to FXAA instead of temporalAA
- [BUGFIX] : Bugfix for excessive gpu memory use.
- [BUGFIX] : Bugfix for Seek to beginning of file playback.
- [BUGFIX] : Bugfix for PixelStreaming within UE5

v0.5.2
------
- [BUGFIX] Bugfix for preview mesh crash in packaged builds.

v0.5.1
------
- [FEATURE ENHANCEMENT] More performant texture uploads
- [BUGFIX] Bugfix for creating packaged builds.
- [BUGFIX] Bugfix for memory corruption during asset load in packaged builds.

v0.5.0
------

- [FEATURE ENHANCEMENT] Adds convience loader for .8iPat local files. 
- [FEATURE ENHANCEMENT] Adds editor preview for assets.
- [FEATURE ENHANCEMENT] Adds new playback controls for custom start/stop times.
- [FEATURE ENHANCEMENT] Adds new playback controls for custom render speed.
- [UI IMPROVEMENT] Reorder asset controls into similar groups.

v0.4.0
------

- [FEATURE ENHANCEMENT] Improves audioless asset render
- [FEATURE ENHANCEMENT] Adds convience methods for asset status

v0.3.2
------

- [BUGFIX] Bugfix for hung playback.

v0.3.0
------

- [FEATURE ENHANCEMENT] Adds normal information to the assets.
- [FEATURE ENHANCEMENT] Adds multiple render modes for assets.


v0.2.0
------

- [FEATURE ENHANCEMENT] Adds PatAsset information to separate data from renderer.

v0.1.0
------

- Initial Release