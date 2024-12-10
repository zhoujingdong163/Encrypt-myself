# Encrypt-myself Documentation in English
[Chinese(中文)](README-CN.md)|English(英文)

## Preamble

We designed this software to better protect the user's data and privacy, and hope to help users encrypt a file more easily and faster through this software, do not use it in illegal ways, and respect our user agreement, thank you!

At present, I (the developer) is in the third year of junior high school, and I may not be able to guarantee the real-time update of the warehouse, please understand!

If you like this project, you can give a star support ✨!

## Introduction

This software is encrypted based on RSA encryption, driven by C++, with the serial number of the drive as the public key, to ensure that users can still recover through our tools in the case of complete loss of data (such as user reinstallation system, driver, etc.) to ensure the security of data.

At the same time, our encryption tool is faster than other tools, and our software can reach up to about $2times10^4byte/s$ under the condition of ensuring the security of your data foundation, provided that your computer should try to avoid other high-computing software occupying system resource space.

And our encryption software is highly secure, requiring that the decryption operation must be on the original encrypted drive (if you really need to, you can back up the data in advance), otherwise our RSA encryption algorithm may decrypt something you don't expect.

Theoretically, all characters that appear in the Ascall code table should be able to be encrypted and decrypted, including Chinese characters.

## Instructions for use

After you discover our project, you can download it through our packaged files, or you can compile it yourself by downloading the source code we distribute.

After the compilation is completed, a '.exe' application will be generated, please name this 'exe' program according to your preferred keyword;

For example, in the next step, the name of my generated application is 'Encrypt-myself.exe', then the keyword referred to by '' in the next program execution is 'Encrypt-myself', that is, when I run the command 'Encrypt-myself -h', a help window will pop up (**you are running cmd or powershell must be in the same directory as the file**).

Tips: It is recommended that you can place this compiled 'exe' file in the 'C:/Windows/system32' directory, which can bring you a better service experience!

### Command description

**Each command should be preceded by \<Name>  arguments, omitted**

`-h` helps

`-l <Word>` login (decryption of files can only be performed after login)

`-e <FilePath> <FileName>` encrypts the 'FileName' file under the absolute path 'FilePath' (note that the file suffix must be added with a suffix)

`-d <FilePath> <FileName>` decrypts the 'FileName' file under the absolute path 'FilePath' (you need to be logged in to do this)
