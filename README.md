# FNAF-SecurityBreach_Chinese
玩具熊的五夜后宫：安全漏洞中文汉化补丁  
This patch can transfer your English language pack of FNAF:Security Breach into Chinese. <br>
## 补丁安装教程
1、下载[fnaf9-WindowsNoEditor_p.pak]()。<br>
2、找到游戏目录中的```Quarters\fnaf9\Content\Paks```文件夹。<br>
3、将下载的```fnaf9-WindowsNoEditor_p.pak```放进去。<br>
4、完成。<br>
## 补丁制作教程
#### 第一步：下载所需文件
UnrealPakSwitch：[下载](./src/UnrealPakSwitchv10.zip)<br>
UnrealLocres：[下载](./src/UnrealLocres.zip)<br>
本体文本：[下载](./src/GameCH.csv)<br>
DLC:RUIN文本：[下载](./src/DLCCH.csv)<br>
本体UE4本地化文件：[下载](./src/Game.locres)<br>
DLC:RUINUE4本地化文件：[下载](./src/DLC.locres)<br>
#### 第二步：使用UnrealLocres将文本打包成UE4本地化文件
1、解压```UnrealLocres```<br>
2、将下载下来的```本体文本```、```本体UE4本地化文件```、```DLC:RUIN文本```、```DLC:RUINUE4本地化文件```也放在```UnrealLocres```的文件夹中。<br>
3、进入```UnrealLocres```的文件夹，打开控制台。win10按住```Shift```+```鼠标右键```然后选择```在此处打开Powershell窗口```，win11```鼠标右键```然后选择```在Windows终端中打开```。<br>
4、在控制台中输入：<br>
```./UnrealLocres.exe ./UnrealLocres.exe import (本体UE4本地化文件名称) (本体文本)```<br>
示例：```./UnrealLocres.exe import Game.locres GameCH.csv```<br>
5、然后回车运行，如果成功，会在文件夹中生成一个叫```Game.locres.new```的文件。<br>
6、DLC文本的方法也是一样的，名称都换成DLC的UE4本地化文件和文本就行了。<br>
#### 第三步：使用UnrealPakSwitch将UE4本地化文件打包成PAK
1、解压```UnrealPakSwitch```<br>
2、在```UnrealPakSwitch```的文件夹找到```fnaf9\Content\Localization\Game\zh-Hans```文件夹，将上一步制作好的本体本地化文件```Game.locres.new```放到这个文件夹然后将文件名改为```Game.locres```。<br>
3、在```UnrealPakSwitch```的文件夹找到```fnaf9\Content\Localization\DLC\zh-Hans```文件夹，将上一步制作好的DLC本地化文件```Game.locres.new```放到这个文件夹然后将文件名改为```Game.locres```。<br>
4、返回```UnrealPakSwitch```文件夹按住鼠标拖动文件夹中的```Pack.txt```到```pack-v11-27.cmd```上，之后会有个报错弹窗直接不用管点确定，如果不出问题的话文件夹中会生成一个叫```newpak.pak```的PAK文件，并且注意文件大小不能是0kb。<br>
#### 第四步：将PAK文件安装到游戏目录
1、打开安全漏洞的游戏目录```Quarters\fnaf9\Content\Paks```，将生成的```newpak.pak```文件放置在这里，并且将名称改为```fnaf9-WindowsNoEditor_p.pak```。<br>
2、完成<br>