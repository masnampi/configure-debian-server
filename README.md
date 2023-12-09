# Configure Debian Server

- 
```
sudo apt update && sudo apt upgrade -y

sudo dpkg-reconfigure tzdata

sudo adduser anonymous
sudo usermod -aG sudo anonymous
su - anonymous
whoami

sudo apt install xfce4 xfce4-goodies xorg dbus-x11 x11-xserver-utils
sudo apt install xrdp
sudo systemctl status xrdp
sudo adduser xrdp ssl-cert
sudo systemctl restart xrdp
sudo apt install ufw
sudo ufw allow from 192.168.1.0/24 to any port 3389

sudo apt install vim nodejs npm htop -y

wget -O chrome.deb https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo apt install ./chrome.deb

wget https://az764295.vo.msecnd.net/stable/6c3e3dba23e8fadc360aed75ce363ba185c49794/code_1.81.1-1691620686_amd64.deb
sudo apt install ./code_1.81.1-1691620686_amd64.deb

https://go.dev/doc/install
```
