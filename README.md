# How To Install Webmin on Ubuntu Server

### Introduction
### Webmin is a modern web control panel that allows you to administer your Linux server through a browser-based interface. With Webmin, you can manage user accounts, configure DNS 
### settings, and change settings for common packages on the fly.
### In this tutorial, you’ll install and configure Webmin on your server and secure access to the interface with a valid certificate from Let’s Encrypt. You’ll then use Webmin to ### add new user accounts, and update all packages on your server from the dashboard.
## Step  — Installing Webmin
## 1. First, update your server’s package index if you’ve not done so recently:
#  sudo apt update && sudo apt upgrade
## 2. Add Webmin Repository
# sudo apt install software-properties-common apt-transport-https
## 3. Add Webmin's GPG key with the following command:
# wget -qO- https://download.webmin.com/jcameron-key.asc | sudo tee -a /etc/apt/trusted.gpg.d/jcameron-key.asc
## 4. Enable the Webmin repository path and add it to your Ubuntu distribution with the following command:
# sudo add-apt-repository "deb [arch=amd64] http://download.webmin.com/download/repository sarge contrib"
## 5. Install Webmin
# sudo apt install webmin
## 6. Checking the status of Webmin as a service in the system
# sudo systemctl status webmin
## 7. Set up firewall and specify TCP port 10000
# sudo ufw allow 10000/tcp
## Adding a Valid Certificate with Let’s Encrypt
## Webmin is already configured to use HTTPS, but it uses a self-signed, untrusted certificate. Let’s replace it with a valid certificate from Let’s Encrypt.
## cNavigate to https://your_domain:10000 in your web browser, replacing your_domain with the domain name pointing to your server’s IP address.
# https://localhost:10000/



- **ScrennShot**:

     ![ScrennShot](https://github.com/abdalazeim/WebminUbuntuServer/blob/main/Webmi.png)



### That's All:
### - Thanks For Usage :)
 ### - Have A Nice Day,GoodBye :)
### >>>>>>> Stashed changes

