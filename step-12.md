#### first you need to install Apache
```
sudo apt install apache2 -y
```
#### then you need to use these commands to start apache
```
sudo systemctl start apache2
```
```
sudo systemctl enable apache2
```
#### then use this command 
```
sudo a2enmod ssl
```
#### then restart using this command
```
sudo systemctl restart apache2
```
#### then create this directory using this command
```
sudo mkdir /etc/apache2/ssl
```
#### then paste this in and replace birkkir with your name
```
sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
    -keyout /etc/apache2/ssl/birkir.local.key \
    -out /etc/apache2/ssl/birkir.local.crt
```
#### afer you have pasted this in you will be asked some questions anser them untull you are asked for a common name then you put in www.yourname.local except replace yourname with your name 
#### then open this file but replace your name with your name 
```
sudo nano /etc/apache2/sites-available/yourname.local.conf
```
#### and type this in but replace birkir with your name
![12](https://github.com/user-attachments/assets/2d37f020-387e-410b-8fb2-828e3a6e0d87)

#### then create this directory using this command and replace yourname with your name 
```
sudo mkdir -p /var/www/html/yourname.local
```
#### the use this command and like always replace yourname with your name 
```
sudo nano /var/www/html/yourname.local/index.html
```
#### then add something like this to the file
![html](https://github.com/user-attachments/assets/8fe61279-632d-4a88-9a1d-3c797626a733)
#### then to apply the changes use these two commands
```
sudo a2ensite yourname.local.conf
```
```
sudo systemctl reload apache2
```
#### for this next step you need to open the client machine
#### on the client machine use this code 
```
sudo nano /etc/hosts
```
#### and add this line
![hosts12](https://github.com/user-attachments/assets/c53f1fce-bce3-451b-8998-ec77323d3cc7)
#### and to confirm that you have it set up go on a web browser and type this in and replace yourname
```
https://www.yourname.local
```
#### and if it shows something like this its working
![website](https://github.com/user-attachments/assets/7dc0df8e-83ab-4d7d-8f61-78c3361fdd9f)











