============================================================
Troubleshooting
============================================================

HVRSound goes out of sync
------------------------------------------------------------

There is a known issue where large jumps ( > 2 seconds ) in time in the HVRActor's HVRAsset time can cause the audio to go out of sync.

Launch from Project Launcher
----------------------------
If launching the build from Project Launcher(Toolbar -> Small arrow next to "Launch" -> Project Launcher), make sure "Advanced" checkbox is turned on and change "Data Build" option from "On the fly" to "By the book". "On the fly" method will delete the HVR content as cache files by mistake so it will trigger a runtime error. That is an known issue.

Undo and Redo
------------------------------------------------------------

Undo and Redo in the editor is not fully implemented.