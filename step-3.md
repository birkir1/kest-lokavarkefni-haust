### for this you need to be in the client machine 
#### the steps for this is very similar to the previous step
#### first you use 
```
sudo hostnamectl set-hostname client1
```
#### to change the hostname to client1
#### then you use 
```
sudo nano /etc/hosts
```
#### and change that file to look something like this
![client-hostname](https://github.com/user-attachments/assets/9a44afe7-67b9-4534-97e2-76ddf4ef18ef)
#### exept replace birkir with your name
#### and then to verify you use
```
hostname -f
```
#### and that shuld output something like this
![client-hostname-verify](https://github.com/user-attachments/assets/9ea5d005-0007-439d-bebb-efe232a42de3)
#### and and you should also use this to verify
```
ping client1."yourname".local
```
#### and that should output something like this
![client-host-name-verify](https://github.com/user-attachments/assets/12f15530-7028-4b49-93c9-a1fc6263f153)
