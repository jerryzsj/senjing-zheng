# How to install Sublime in Ubuntu

## Step 1
### Install dependencies: 

```bash
sudo apt-get update
sudo apt install dirmngr gnupg apt-transport-https ca-certificates software-properties-common
```

## Step 2:
### Add apt-key into the apt-repository
```bash
curl -fsSL https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
sudo add-apt-repository "deb https://download.sublimetext.com/ apt/stable/"
```

## Step 3: 
### update and install sublime
```bash
sudo apt-get update
sudo apt install sublime-text
```

## Enjoy
