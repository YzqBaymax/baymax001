# Git Bash 使用教程

## 一、简介
Git Bash 是一款基于 MSYS2 的 Bash shell 环境，专门为 Windows 用户提供了便捷的 Git 命令行工具。通过 Git Bash，您可以直接在 Windows 上使用 Git 命令以及许多 Linux/Unix 常用的 shell 工具，极大地简化了版本控制工作流程。本教程将介绍一些 Git Bash 的基本使用方法。

## 二、安装与启动

1. **安装 Git for Windows**：
   访问 [Git 官方下载页面](https://git-scm.com/downloads) 下载适用于 Windows 的安装包，按照向导进行安装，确保勾选 "Git Bash Here" 选项。

2. **启动 Git Bash**：
   - 右键点击任意文件夹，选择 "Git Bash Here"，将在该目录下打开 Git Bash。
   - 或者，通过开始菜单找到 "Git Bash" 并点击启动。

## 三、基本命令示例   
（提示：在实际操作时，不要复制代码块中的 $ 符号，它是命令行提示符的表示，仅用于标识命令的起始位置）

??? 查看当前工作目录
    使用 `pwd` 命令查看当前所在目录：  
    ```bash  
    $ pwd  
    /home/user  

??? 切换工作目录
    使用`cd` 命令切换工作目录：      
    $ cd /path/to/directory  

??? 列出当前目录下的文件和目录
    使用`ls` 命令列出当前目录下的文件和目录：
    $ ls
    file1.txt  file2.txt  directory1  directory2

??? 创建目录与文件
    使用`mkdir` 命令创建目录：  
    $ mkdir new_directory   
    使用`touch` 命令创建文件：   
    $ touch new_file.txt

??? 删除目录与文件
    使用`rm` 命令删除文件：     
    $ rm file.txt  
    使用`rm -r` 命令删除目录及其内容：     
    $ rm -r directory  

??? 移动或重命名文件或目录
    使用`mv` 命令移动或重命名文件或目录：    
    $ mv old_file.txt new_file.txt  
    $ mv old_directory new_directory

??? 复制文件或目录
    使用`cp` 命令复制文件或目录：    
    $ cp file.txt new_file.txt  
    $ cp -r directory new_directory

??? 查看文件内容
    使用`cat` 命令查看文件内容：    
    $ cat file.txt   
    This is a sample file.   
    使用`less` 命令查看文件内容：       
    $ less file.txt  
    This is a sample file.  
    使用`head` 命令查看文件开头的几行：       
    $ head -n 5 file.txt   
    This is a sample file.  
    使用`tail` 命令查看文件结尾的几行：      
    $ tail -n 5 file.txt  
    This is the last line.  
    使用`grep` 命令查找文件中的指定内容：      
    $ grep "pattern" file.txt  
    This is a sample file.  
    使用`find` 命令查找指定目录下的文件或目录：      
    $ find /path/to/directory -name "*.txt"  
    /path/to/directory/file1.txt  
??? 实时查看网页调试
    $ mkdocs serve    
    ctrl + c终止

## 四、Git 基本操作

### 1. 初始化 Git 仓库
使用`git init` 命令初始化一个 Git 仓库：    
$ git init
初始化成功后，当前目录将变为 Git 仓库。

### 2. 添加文件到暂存区
使用`git add` 命令将文件添加到暂存区：    
$ git add file.txt
使用`git add .` 命令将当前目录下的所有文件添加到暂存区：    
$ git add .

### 3. 提交更改到本地仓库
使用`git commit` 命令提交更改到本地仓库：  
$ git commit -m "commit message"







