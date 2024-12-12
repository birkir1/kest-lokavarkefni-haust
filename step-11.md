#### first you need to install ssh using this command
```
sudo apt install openssh-server -y
```
#### then you need too open this file 
```
sudo nano /etc/ssh/sshd_config
```
#### and add this to it
![11](https://github.com/user-attachments/assets/f4a95937-1f78-45d0-8bcf-7bb960b07544)
#### then you save and exit the file 
#### and restart the ssh using this command
```
sudo systemctl restart ssh
```
