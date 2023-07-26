# FNAF-SecurityBreach_Chinese
玩具熊的五夜后宫：安全漏洞中文汉化补丁  
This patch can transfer your English language pack of FNAF:Security Breach into Chinese. <br>
## 补丁制作教程
#### 第一步：下载所需文件
UnrealPakSwitch：<br>
UnrealLocres：<br>
本体文本：<br>
DLC:RUIN文本：<br>
本体UE4本地化文件：<br>
DLC:RUINUE4本地化文件：<br>
#### 第二步：使用UnrealLocres将文本打包成UE4本地化文件
1、解压```UnrealLocres```，并新建一个文件夹将```UnrealLocres.exe```放进去。<br>
2、将下载下来的```本体文本```、```本体UE4本地化文件```、```DLC:RUIN文本```、```DLC:RUINUE4本地化文件```也放在新建的文件夹中。<br>
3、进入新建的文件夹，打开控制台。win10按住```Shift```+```鼠标右键```然后选择```在此处打开Powershell窗口```，win11```鼠标右键```然后选择```在Windows终端中打开```。<br>
4、在控制台中输入：<br>
```./UnrealLocres.exe ./UnrealLocres.exe import ```<br>
注意空格！之后先把```本体UE4本地化文件```按住拖动到控制台中，然后空格再把```本体文本```拖入控制台中。<br>
示例（不要照搬！）：<br>
```./UnrealLocres.exe import D:\ProgramFiles\UnrealPakSwitchv10\UnrealLocres\Game.locres D:\ProgramFiles\UnrealPakSwitchv10\UnrealLocres\GameCH.csv```<br>
5、然后回车运行，如果成功，会在