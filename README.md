按照原始仓库教程在 15.0.1 patch 了一下，也许能用？起码第一天是好的

# 010_Editor_crack
010 Editor v11.01编辑器破解版，破解教程

#### 使用方法：

官网下载30天试用版，链接：

https://www.sweetscape.com/download/010EditorWin64Installer.exe

一步步安装，将`010Editor_crack.exe`重命名，复制到安装的根目录并覆盖原文件，

启动，点击Register，输入任意字符，点击Check License，注册成功

![image-20210508104423061](img/image-20210508104423061.png)

![image-20210508104445279](img/image-20210508104445279.png)

#### 破解教程

shift+f12过滤字符串`invalid name`  

![image-20210508105413251](img/image-20210508105413251.png)

ctrl +x 定位关键函数

![image-20210508105447213](img/image-20210508105447213.png)

分析sub_1401E3F30()发现

关键赋值v11  当等于0xDB时，注册成功

![img](img/1618815351854-87713558-0da3-4e84-b167-9b1bc71cd143.png)

使用keypatch修改为

mov eax,0xdb

ret

![img](img/1618815933898-6d6544c6-8199-4e5b-81ac-57c67d3c073f.png)

