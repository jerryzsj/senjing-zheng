# How to setup WSL2 in windows

## Step 1: 
### Open PowerShell with Admin and run: 
```bash
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
## Step 2: 
### Reboot, Open PowerShell with Admin and run: 
```bash
wsl --set-default-version 2
```
#### run wsl_update_x64.msi

## Step 3: 
### Install Ubuntu20.04 via wsl
```bash
wsl --install -d ubuntu-20.04
```

## Step 4:
### Modify default DNS setting 
'''
sudo nano /etc/resolv.conf
'''
#### change the nameserver into: 8.8.8.8

## Step 5:
### Update the Ubuntu with
'''
sudo apt-get update
'''

## Enjoy

https://askubuntu.com/questions/1364984/dns-not-working-on-wsl


install sublime:
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
sudo apt install apt-transport-https
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt update
sudo apt install sublime-text