#### first you run this command to install samba
```
sudo apt install samba -y
```
#### then you run this command 
```
sudo mkdir -p /srv/samba/{IT,Management,Finance}
```
#### and then you run these commands
```
sudo chown -R :tolvudeild /srv/samba/IT
```
```
sudo chown -R :Stjornun /srv/samba/Management
```
```
sudo chown -R :Sala /srv/samba/sales
```
```
sudo chmod -R 770 /srv/samba/IT
```
```
sudo chmod -R 770 /srv/samba/Management
```
```
sudo chmod -R 770 /srv/samba/sales
```
```
sudo setfacl -m g:tolvudeild:rwx /srv/samba/*
```
```
sudo setfacl -m g:Stjornun:rwx /srv/samba/*
```
#### and then you open this file
```
sudo nano /etc/samba/smb.conf
```
#### and add this to it
![IT](https://github.com/user-attachments/assets/1af8af86-fb8e-4456-9294-4898eff84ad8)
![stjorn](https://github.com/user-attachments/assets/2a358c07-5e7e-4939-a08f-b68878900066)
![Sala](https://github.com/user-attachments/assets/379e51cd-255f-4b9c-afaf-d30723c3a32f)
#### then you restart semba using these command 
```
sudo systemctl restart smbd
```
```
sudo systemctl enable smbd
```
#### then do this to every user and replase the xxx with the username
```
sudo smbpasswd -a xxx
```




