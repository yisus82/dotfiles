Software
========

* Android Studio
* Eclipse
* Git
* Google Chrome
* Java
* K-Lite Codec Pack
* Mega Sync
* Meld
* Mozilla Firefox
* MS Edge
* MS Office
* PyCharm
* Python
* QBittorrent
* Spotify
* Sublime Text
* Team Viewer
* Unity
* VS Code Insiders
* WinRAR

Customization of Powershell
===========================

Installing Chocolatey
---------------------

* Open Powershell and run the following command:
```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

Installing Fira Code / Fira Code NF in Windows
----------------------------------------------

* Open Powershell and run the following commands:
```powershell
choco install firacode
```
```powershell
choco install firacodenf
```

Installing oh-my-posh
---------------------

* Open Powershell and run the following commands:
```powershell
Install-Module posh-git -Scope CurrentUser
```
```powershell
Install-Module oh-my-posh -Scope CurrentUser
```
```powershell
Set-Prompt
```
```powershell
Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck
```
```powershell
if (!(Test-Path -Path $PROFILE )) { New-Item -Type File -Path $PROFILE -Force }
notepad $PROFILE
```

* Append the following lines to PowerShell profile:

```powershell
Import-Module posh-git
Import-Module oh-my-posh
Set-Theme Agnoster
```

Installation of Ubuntu WSL
==========================

* Open Powershell and run the following commands:
```powershell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
```powershell
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
```powershell
wsl --set-default-version 2
```

* Restart PC, open Microsoft Store and install Ubuntu


Installation and customization of Windows Terminal
==================================================

* Open Microsoft Store and install Windows Terminal

* Copy settings.json


Installing Fira Code in WSL
---------------------------

* Open Windows Terminal and run the following commands:
```shell
sudo add-apt-repository universe
```
```shell
sudo apt update
```
```shell
sudo apt install fonts-firacode
```

Installation and setup of zsh and Oh-my-zsh
-------------------------------------------

* Open Windows Terminal open and run the following commands:
```shell
sudo apt-get install zsh
```
```shell
sudo apt-get install build-essential
```
```shell
sudo apt install ruby ruby-dev ruby-colorize
```
```shell
sudo gem install colorls
```
```shell
sudo add-apt-repository ppa:dawidd0811/neofetch && sudo apt update && sudo apt install neofetch
```
```shell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
```shell
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
```shell
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
```shell
git clone https://github.com/lukechilds/zsh-nvm.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-nvm
```
```shell
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

* Copy .zshrc and .p10k.zsh to home directory

* Generate SSH key and add it to Github account
