#### to configure a static ip with a privite interface first you use 
```
ifconfig 
```
and it should look something like this
![ifconfig](https://github.com/user-attachments/assets/e70e1a7a-8f1d-4329-9960-2e61051e2bd7)
#### then for me i take the second number the ens37 and i put it in the network interfaces file and to access it you use 
```
sudo nano /etc/network/interfaces 
```
#### and in there you change it to look something like this
![privite-interface](https://github.com/user-attachments/assets/eef5740b-6a3e-4bb7-8158-a7ea266f6f86)
#### then you save and quit
#### after that you use 
```
sudo systemctl restart networking
```
#### to restart the network
#### and then you should have the ip configured but if you want to test it use
```
ip addr show eth1
```
#### and somewere in the output it should show 
#### inet 192.168.1.1/24
