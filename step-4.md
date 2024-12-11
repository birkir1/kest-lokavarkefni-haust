#### first you install the ISC-DHCP-Server using this command 
```
sudo apt install isc-dhcp-server -y
```
#### then you open this file 
```
sudo nano /etc/dhcp/dhcpd.conf
```
#### and you change this to be like this
![DHCP](https://github.com/user-attachments/assets/ed1342bb-518b-40df-8b50-020bf811946c)
#### then you open this 
```
sudo nano /etc/default/isc-dhcp-server
```
#### and for me i changed it to be like this 
![interfaces](https://github.com/user-attachments/assets/70f5efe7-ed07-47cb-99b6-dfa779fdbe5f)
#### and in the end you use these to restart the server
```
sudo systemctl restart isc-dhcp-server

```
```
sudo systemctl enable isc-dhcp-server
```
#### and then u use this to check if its running 
```
sudo systemctl status isc-dhcp-server
```
#### and it shuld look some thing like this
![server](https://github.com/user-attachments/assets/79be2524-0422-4d61-80cc-25c14d01110a)
