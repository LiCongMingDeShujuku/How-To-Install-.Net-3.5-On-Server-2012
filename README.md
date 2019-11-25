![CLEVER DATA GIT REPO](https://raw.githubusercontent.com/LiCongMingDeShujuku/git-resources/master/0-clever-data-github.png "李聪明的数据库")

# 如何在Server 2012上安装.Net 3.5
#### How To Install .Net 3.5 On Server 2012
**发布-日期: 2016年3月7日 (评论)**

![#](images/##############?raw=true "#")

## Contents

- [中文](#中文)
- [English](#English)
- [Build Info](#Build-Info)
- [Author](#Author)
- [License](#License) 


## 中文
以下是如何在Server 2012上安装.Net 3.5。不可否认，尝试通过服务器管理器在Server 2012上安装good'ole .net 3.5是一件非常痛苦的事。以下是一些快速入门的步骤。


1. 打开命令提示符“As Administrator”。

2. 运行此脚本（不必修改任何内容）。这将设置功能安装，以允许你选择其他来源，如文件，CD，已安装的驱动器等。

3. 接下来返回操作系统并找到服务器安装文件（可能是网络共享上的.iso），并将驱动器“mount”设为cd，或者将所有安装文件复制到服务器上。
注意：你可以从网络安装.iso文件。只是需要一分多钟运行.net 3.5安装程序。

4. 运行服务器管理器，然后再次导航到.NET 3.5选择。你会注意到在你选择它并单击“Next”后，会看到提示“specify an alternate source path”。

5. 浏览SXS文件夹`＃\ Sources \ SXS`

6. 单击“安装”。

在这之后最好可以重启服务器，以确保操作系统获取更改，当然也会撤消'mount'。否则你将锁定.iso阻止其他人使用它。


## English
Here’s how to install .Net 3.5 on Server 2012. Admittedly it’s a real pain trying to get the good’ole .net 3.5 installed on Server 2012 through server manager. Here are some quick steps to get you started.

1. Open Command Prompt ‘As Administrator’.

2. Run this script ( you don’t have to modify anything ). This sets up the feature installation to allow you to select other sources such as files, cd’s, mounted drives, etc.
dism /online /enable-feature /featurename:NetFX3 /all /Source:d:\sources\sxs /LimitAccess

3. Next go back to the OS and find the Server install files (probably .iso on network share), and ‘mount’ the drive as a cd, or copy all the installation files over to the server locoally.
Note: You can mount .iso files from the network. Just takes a minute longer to run the .net 3.5 install.

4. Run through the Server Manager, and navigating to the .NET 3.5 selection again. You’ll noticed down below after you’ve selected it and clicked ‘Next’ you’ll see the ‘specify an alternate source path’.


5. Browse to the SXS folder `#\Sources\SXS`

Done.

Might be a good idea to restart the server afterwords to ensure the OS picks up the changes, and of course will undo the ‘mount’. Otherwise you’ll lock the .iso and keep others from using it.



[![WorksEveryTime](https://forthebadge.com/images/badges/60-percent-of-the-time-works-every-time.svg)](https://shitday.de/)

## Build-Info

| Build Quality | Build History |
|--|--|
|<table><tr><td>[![Build-Status](https://ci.appveyor.com/api/projects/status/pjxh5g91jpbh7t84?svg?style=flat-square)](#)</td></tr><tr><td>[![Coverage](https://coveralls.io/repos/github/tygerbytes/ResourceFitness/badge.svg?style=flat-square)](#)</td></tr><tr><td>[![Nuget](https://img.shields.io/nuget/v/TW.Resfit.Core.svg?style=flat-square)](#)</td></tr></table>|<table><tr><td>[![Build history](https://buildstats.info/appveyor/chart/tygerbytes/resourcefitness)](#)</td></tr></table>|

## Author

- **李聪明的数据库 Lee's Clever Data**
- **Mike的数据库宝典 Mikes Database Collection**
- **李聪明的数据库** "Lee Songming"

[![Gist](https://img.shields.io/badge/Gist-李聪明的数据库-<COLOR>.svg)](https://gist.github.com/congmingshuju)
[![Twitter](https://img.shields.io/badge/Twitter-mike的数据库宝典-<COLOR>.svg)](https://twitter.com/mikesdatawork?lang=en)
[![Wordpress](https://img.shields.io/badge/Wordpress-mike的数据库宝典-<COLOR>.svg)](https://mikesdatawork.wordpress.com/)

---
## License
[![LicenseCCSA](https://img.shields.io/badge/License-CreativeCommonsSA-<COLOR>.svg)](https://creativecommons.org/share-your-work/licensing-types-examples/)

![Lee Songming](https://raw.githubusercontent.com/LiCongMingDeShujuku/git-resources/master/1-clever-data-github.png "李聪明的数据库")

