============
Known Issues
============

HVRSound goes out of sync
------------------------------------------------------------

There is a known issue where large jumps ( > 2 seconds ) in the ``HRActor``'s time can cause the audio to go out of sync.

Undo/Redo
---------
Undo and Redo functionality on ``HvrActor`` is not fully implemented.

Lighting and Shadowing
----------------------
There is no support of lighting or shadowing on the ``HvrActor`` at the moment.

VEP Codec Support
-----------------
As Unreal Engine doesn't support OpenGL on Windows, there's no VEP support on Windows Unreal Engine.