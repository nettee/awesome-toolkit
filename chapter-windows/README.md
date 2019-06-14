# Windows 配置

## 显示

下载字体并双击 ttf 文件安装即可。

等宽字体推荐 [Inconsolata](https://fonts.google.com/specimen/Inconsolata)。

## 远程连接服务器

Windows 一般不作为运行环境，要远程连接到 Linux 机器。

SSH 登录使用 putty，[putty 配色方案](https://github.com/chriskempson/tomorrow-theme)（需要导入注册表）。

SCP 文件传输使用 putty 自带的命令 `pscp`

```cmd
:: -C 表示允许压缩传输

:: 文件会传到 ~
pscp -C c:\local\file.txt username@server:.

:: 文件会传到 ~/remote/dir
pscp -C c:\local\file.txt username@server:remote/dir 

pscp -C username@server:remote/file.tar.gz c:\local\dir
```
