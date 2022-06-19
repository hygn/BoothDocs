# VRC System Monitor Manual
## -1. READ PRECAUTIONS
[https://booth.hygn.moe/SystemMonitor/Precautions.html](https://booth.hygn.moe/SystemMonitor/Precautions.html)
## 0. Import liltoon shader to your Unity project
If liltoon shader is not in your Unity project, you must import liltoon shader first.
## 1. Import Unitypackage to your Unity project
![](./ManualAssets/importprefab.png)
## 2. Drag prefab into avatar root
![](./ManualAssets/dragprefab.png)
## 3. Uncheck "Is Active" in parent constraints
![](./ManualAssets/disableparentconstraints.png)
## 4. Adjust position of prefab 
![](./ManualAssets/changetransform.png)
## 5. Assign left lower arm bone to parent constraints
![](./ManualAssets/armboneassign.png)
## 6. Click "Activate" in parent constraints
![](./ManualAssets/activateconstraints.png)
## 7. Disable prefab in inspector
![](./ManualAssets/disableprefab.png)
## 8. Open FX layer of your avatar
![](./ManualAssets/selectfxlayer.png)
## 9. Add parameters to FX layer
![](./ManualAssets/addparams.png)\
**All parameters are case-sensitive.**
* SysStatus_percent (float)
* SysStatus_sync1 (bool)
* SysStatus_sync2 (bool)
* SysStatus_sync3 (bool)
## 10. Add two layers into FX layer
![](./ManualAssets/addlayer.png)
## 11. Set layer weight to 1
![](./ManualAssets/setweight.png)
## 12. Copy animation controller from provided example controller and paste into FX layer
![](./ManualAssets/examplecontrollertofx.png)
## 13. Set "TDD_Base" state into default state
![](./ManualAssets/setdefault.png)
## 14. repeat 12,13 with "SysStatusControl" layer
*If you want to turn on or off with Expression Menu, it is recommended to make an idle state in the FX layer first and paste the example controller.*\
![](./ManualAssets/secondlayer.png)
## 15. Add parameters into Expression Parameter
![](./ManualAssets/exparam.png)
## 16. Start contained VRC_SysStatus_GUI.exe
![](./ManualAssets/OSCSoftware.png)\
*Configure software according to Software Manual*
## 17. Reset OSC settings in VRChat after upload and check OSC is working properly
![](./ManualAssets/resetosc.png)
![](./ManualAssets/OSCdebug.png)