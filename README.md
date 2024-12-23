# Encrypt-myself 中文文档

Chinese(中文)|[English(英文)](README-EN.md)

## 序言

我们设计本软件的目的是为了能够更好的保护用户的数据和隐私，希望可以通过本软件去帮助用户更加轻易更加快捷的加密某个文件，请勿将其用于非法途径，并尊重我们的用户协议，感谢！

目前本人（开发者）在初三，不一定能够保证仓库的实时更新，敬请谅解！

如果您喜欢本项目，可以给个 star 支持一下哦✨！

## 介绍

本软件基于 RSA 加密方式进行加密，由 C++ 驱动，以驱动器的序列号作为公钥，保证用户在彻底丢失数据的情况下（如用户重装系统、驱动等）仍旧能够通过我们的工具去进行恢复，保证数据的安全。

同时我们的加密工具速度较其它工具速度较快，在保证您的数据基础安全的情况下，我们的软件最高可以达到 $2\times10^4byte/s$ 左右，前提是您的电脑应尽量避免其它高运算量的软件占用系统资源空间。

并且我们的加密软件安全度极高，要求必须要在原加密驱动器上才可进行解密操作（如果您的确有需要，可以提前将数据进行备份），否则我们的 RSA 加密算法解密出来可能会出现令您意想不到的内容。

理论上出现在了 Ascall 码表的字符都应可以被加密和解密，包括中文字符。

## 使用说明

您在发现我们的项目之后，可以通过我们打包好的文件进行下载，也可以通过下载我们下发的源代码自行编译。

编译完成后，会生成一个 `.exe` 应用程序，请按照您喜好的关键字为这个 `exe` 程序命名；

例如在接下来的步骤中我的生成的应用程序名为 `Encrypt-myself.exe` ，那么接下来的程序执行中 `<Name>` 所指的关键字就是 `Encrypt-myself` ，即当我运行命令 `Encrypt-myself -h` 时，会弹出帮助窗口（**您运行的 cmd 或者 powershell 必须与文件处于同一目录下**）。

温馨提示：建议您可以将此编译好的 `exe` 文件放置在 `C:/Windows/system32` 目录下，这样可以为您带来更好的服务体验！

### 命令说明

**运行每个命令前应当加上 \<Name> 参数，下略**

`-h` 帮助

`-l <Word>` 登录（登录后才能进行文件的解密操作）

`-e <FilePath> <FileName>` 加密绝对路径 `FilePath` 下的 `FileName` 文件（注意有文件后缀的一定要加后缀）

`-d <FilePath> <FileName> ` 解密绝对路径 `FilePath` 下的 `FileName` 文件（您需要登录后才能进行此操作）

