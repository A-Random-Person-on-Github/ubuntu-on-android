# ubuntu-on-android
A tweaked ubuntu-21.04 with xfce4 runs on android with termux/proot-distro

![stage](https://img.shields.io/badge/Status-Testing-orange)

its called `hippo`

### A note before you try
- This is a more like a stock xfce4 with some tweaks.
- As lot of it is preinstalled you can login and start right after you install 
- And its in early stages of building so things may look kind of bad (make sure to notice me if you find any in issues)
- If you have any issues or suggestions make sure i know at https://github.com/RandomCoderOrg/ubuntu-on-android/issue (create an issue)

# installation
```bash
# install dependencies
apt update; apt upgrade -y ; apt install -y pulseaudio proot-distro git -y
# clone the code
git clone https://github.com/RandomCoderOrg/ubuntu-on-android
# run the installer
cd ubuntu-on-android
bash install.sh
# install
proot-distro install hippo --user  ubuntu
```
## logging into hippo
```bash
# run
proot-distro login hippo
```
## starting vncserver
```bash
vncserver :1
```
## stoping vncserver
```bash
vncserver --kill :1
```
## Logout from hippo :)
```bash
exit
```
### Default passwords
`user` -> ubuntu



user password -> `ubuntu`


you can change by command `passwd`


vnc password -> `ubuntu`


you can change it by command `vncpasswd`


## More updates comming soon👊.
