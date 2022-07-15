# How to setup WSL2 in windows

## Step 1

### Open PowerShell with Admin and run: 
### dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

## Step 2: To set the default WSL version as WSL2:
### wsl --set-default-version 2

## Step 3: Download Ubuntu20.04 and install
### wsl --install -d ubuntu-20.04

## Enjoy