## Installation from pre-build

### Docker: linux / macOS (m1 supported)

Special thanks to [Trinketer22](https://github.com/Trinketer22/) contributor we have Docker image with docker-hub:

1. Docker-hub pre-build images can be founded [here](https://hub.docker.com/r/trinketer22/func_docker/)
2. Docker files with instructions can be founded [here](https://github.com/Trinketer22/func_docker)

### Linux / macOS (intel)

1. Download needed special pre-builds (from SpyCheese repo) for
   Linux : [here](https://github.com/SpyCheese/ton/actions/runs/2585669126), for
   Mac : [here](https://github.com/SpyCheese/ton/actions/runs/2618664609)
    1. You need to be logged-in to GitHub to download pre-builds
2. Install `Python3.9` or higher
3. Run `pip install toncli` or `pip3 install toncli`
    1. If you see `WARNING: The script toncli is installed in '/bla/bla/bla/Python/3.9/bin' which is not on PATH.`
       please manually add absolute `bin` path to PATH env
4. Run `toncli` and pass absolute path to `func` / `fift` / `lite-client` from first step

### Windows

1. You need to download the latest version of python (3.9+) from the official website, you can do
   this [here](https://www.python.org/downloads/)
    1. Please, **don't** install Microsoft Store version. It will not work.
2. During installation, on the first screen, you need to click the "Add Python to PATH" checkbox, this is very
   important!

![image](https://user-images.githubusercontent.com/19264196/160259049-8ed99862-a765-4653-84cb-b6818c0aa0b3.png)

3. After successful installation, open the console (you can do this by pressing `Win+X`, selecting `Windows Terminal` in
   the menu)

4. Install `toncli` by running `pip install toncli`

5. Download the compiled TON binaries from [here](https://github.com/SpyCheese/ton/actions/runs/2618774052) (you need to
   be logged in to GitHub)

![image](https://user-images.githubusercontent.com/19264196/160259203-07fd0e26-9b8e-4aff-b4f0-8e4e6f871088.png)

6. Unzip the downloaded archive

7. Add [libcrypto-1_1-x64.dll](https://disk.yandex.ru/d/BJk7WPwr_JT0fw) to unziped files

![image](https://user-images.githubusercontent.com/19264196/160259288-3af468d7-74ac-45cb-9001-9f2604cf4119.png)

9. Open the folder in the console (right mouse button, open in the terminal in Windows 11, Windows 10 and less - copy
   the path in Explorer and in the PowerShell (win+x) and run `cd <<copied path>>`)

10. Run `toncli` in console, it will automatically detect `.exe` files and added paths to config:

![image](https://user-images.githubusercontent.com/19264196/160259355-dacc0234-f8b7-4b9e-b1cd-8a5d6df0712a.png)

11. Success!

## Installation from source

### Linux & macOS

1. Follow official [docs](https://ton.org/docs/#/compile) to compile sources
    1. If you use arch linux you may use [AUR package](https://aur.archlinux.org/packages/ton-git) (please keep in mind
       that you need compile SpyCheese repo toncli-local branch
       => [https://github.com/SpyCheese/ton/tree/toncli-local](https://github.com/SpyCheese/ton/tree/toncli-local))
2. Run `pip install toncli` or `pip3 install toncli`
    1. If you see `WARNING: The script toncli is installed in '/bla/bla/bla/Python/3.9/bin' which is not on PATH.`
       please manually add absolute `bin` path to PATH env
3. Run `toncli` and pass absolute path to `func` / `fift` / `lite-client` from first step


