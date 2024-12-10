#### first you use 
```
sudo hostnamectl set-hostname server1
```
#### to change the hostname to server1
#### then you use 
```
sudo nano /etc/hosts
```
#### and change that file to look something like this
![hostname](https://github.com/user-attachments/assets/bab6616c-1c38-4169-9979-5629bcbd25a2)
#### exept replace birkir with your name
#### then to verify tyou use
```
hostname -f
```
#### and that should output something like this
![hostname-f](https://github.com/user-attachments/assets/c1bb6ed3-2dea-4ee9-91d3-12ce25d4bd0a)
#### and and you should also use this to verify
```
ping server1."yourname".local
```
#### and that should output something like this
![hostname-verify](https://github.com/user-attachments/assets/6f0d0ffb-e123-4f88-9f5f-340b706d1eb0)
