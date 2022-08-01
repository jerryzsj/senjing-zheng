# How to install sublime in Ubuntu

## Step 1

### Install dependencies: 

```bash
sudo apt-get update
sudo apt install dirmngr gnupg apt-transport-https ca-certificates software-properties-common
```

## Step 2: To generate ssh-key:

ssh-keygen

## Step 3: Reboot

## Step 4: Add ssh-key into the ssh-agent

ssh-add $SSH-KEY-NAME$

## Enjoy


<!-- $ ssh-agent /bin/sh
$ ssh-add $yourkey -->