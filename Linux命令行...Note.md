# chapter 3
[TOC]
-  **shell**: 什么是shell?
-  **bash**: 什么是bash? 
-  **man命令**
-  **Linux目录**
-  **cp命令**
-  **ls命令**
-  **创建文件touch命令**
-  **链接文件**
-  **移动（重命名）mv**
-  **删除文件rm命令**
-  **创建目录命令mkdir**
-  **删除目录rmdir**
-  **查看文件统计信息stat**
-  **查看文件类型信息file**
-  **查看整个文件命令cat, more, less,其中less最好用**
-  **查看文件的一小部分tail和head命令**
-  **探测进程ps**
-  **实时监测进程top**
-  **结束进程kill**
## shell
## bash
## man
>用于查找shell命令以及GNU在线手册<br>
Usage：<br>
**man [OPTION]**<br>
**man date** 查看date命令的用法<br>
## Linux目录
## 移动（重命名）mv
> 需要注意移动有软链接指向的文件会有**麻烦**, **mv**比**cp**速度快
## 删除文件rm命令
> 关于删除带链接的文件（Page 66），最好使用**rm -i file**命令，这增加了确定删除步骤，因为这条命令删除的文件无法找回（bash shell 中没有回收站）
## 删除目录rmdirz
> 只删除空目录，若是目录中有文件则不会删除这个目录, 简单的**rm**也无法删除目录，若是真想删除整个目录可以采用**rm -ff directory**删除整个directory目录，但是这个命令要慎用，特别是`root`账户登录时。

## 实时监测进程top
> 主要查看%cpu和%MEM，分别对应cup占用率和内存占用率,PID是进程号
## 结束进程kill
Usage:<br>
** kill [options]**<br>
** kill 3940** 结束进程号为3490的进程
