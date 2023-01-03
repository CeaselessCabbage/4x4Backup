This version is a lightly updated version of 4x4 Evolution to fix some critical issues on February 21, 2019

========================================
BUG FIX 1
========================================
Issue Resolved:
-Fixes menus delay

What was the issue:
-Function GetPerformanceFrequency() has a bug that can cause delay of several seconds when moving between menus, and using in-game chat

Fix:
-Changed 4x4.exe offset 0x19AE87 from 01 to 00 to force use of lower precision timer
-Changed 4x4ed.exe offset 0x1F3E77 from 01 to 00 to force use of lower precision timer

Potential problem:
This fix may break the game on anything running WinME or lower. Run the Win9x executable for those of you partying like it's Y2K.


========================================
BUG FIX 2
========================================
Issue Resolved:
-Fix master server connection delays. Prevents issue with multiple failed retries when connecting online

What was the issue:
-4x4evolution.com is not available for purchase

Fix:
-Changed 4x4.exe offset 0x1CD4E1 to use 4x4evolution.net instead
-Changed 4x4ed.exe offset 0x1CD4D4 to use 4x4evolution.net instead
-Patch is applied to both versions

Potential problem:
None, loss of 4x4evolution.com will occur at some point.

