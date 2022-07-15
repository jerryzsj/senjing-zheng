# How to setup WSL2 in windows

## Step 1: 
### Open PowerShell with Admin and run: 

#### dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
#### dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

## Step 2: 
### Reboot, Open PowerShell with Admin and run: 

#### wsl --set-default-version 2
#### run wsl_update_x64.msi

## Step 3: 
### Install Ubuntu20.04 via wsl

#### wsl --install -d ubuntu-20.04

## Enjoy