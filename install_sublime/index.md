# How to setup SSH in windows

## Step 1

### Open PowerShell with Admin and run: 

Get-Service ssh-agent | Set-Service -StartupType Automatic -PassThru | Start-Service

## Step 2: To generate ssh-key:

ssh-keygen

## Step 3: Reboot

## Step 4: Add ssh-key into the ssh-agent

ssh-add $SSH-KEY-NAME$

## Enjoy


<!-- $ ssh-agent /bin/sh
$ ssh-add $yourkey -->