# Install GUI on Ubuntu Server  

### First update your system
```
sudo apt update
```
### Install the tasksel utility
```
sudo apt install tasksel
```
### Install the slim display manager because it is lightweight   
```
sudo apt install slim
```
### Check the current display manager   
```
cat /etc/X11/default-display-manager 
```
### Install the desktop environment
```
sudo tasksel
```
then select 
```
LXDE desktop
```
### Install the Tigervnc server to visualize your GUI
```
sudo apt install tigervnc-standalone-server
```
### To run the session 
```
vncserver -localhost no
```
and set the password to access the GUI
### To display active session 

```
vncserver -list
```
### Open the inbound port 5900 from the ec2 security group

### Open tigervnc app and add the 

```
instancepublicIP::5902
```
