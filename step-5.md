#### first you install bind using this command
```
sudo apt install bind9 -y
```
#### and then you open this file and change it to look something like this
```
sudo nano /etc/bind/named.conf.local
```
#### and change it to look something like this
![bindfile](https://github.com/user-attachments/assets/6279ca1b-62fd-4d37-a40e-7d5ba13dc4ef)
#### and then you open this 
```
sudo nano /etc/bind/zones/birkir.local.db
```
#### and change it to be something like this
![bind-zone1](https://github.com/user-attachments/assets/c778dc50-b096-4244-8807-013aa5e9bc37)
![bind-zone2](https://github.com/user-attachments/assets/dc882376-a565-4f6c-8856-23854ee5d6c0)
#### and then you open this file
```
sudo nano /etc/bind/zones/rev.3.2.1.in-addr.arpa
```
#### and change it to be something like this
![bind-zones](https://github.com/user-attachments/assets/d37d8970-edce-4fb4-a5e2-c31f3d2c6784)
#### and then you restart using these 
```
sudo systemctl restart bind9
```
```
sudo systemctl enable bind9
```
