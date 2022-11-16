## DOCUMENTATION OF LOAD BALANCER SOLUTION WITH APACHE


`sudo apt update`
![apt update status](./Images/apt%20update%20status.png)
`sudo apt install apache2 -y`
![apache status](./Images/apache%20status.png)
`sudo apt-get install libxml2-dev`
![libxml2-dev status](./Images/libxml2-dev%20status.png)
`ENABLING MODULES COMMANDS USED:`

`sudo a2enmod rewrite`

`sudo a2enmod proxy`

`sudo a2enmod proxy_balancer`

`sudo a2enmod proxy_http`

`sudo a2enmod headers`

`sudo a2enmod lbmethod_bytraffic`

![modules status](./Images/modules%20status.png)

`sudo systemctl status apache2`
![systemctl apache status](./Images/systemctl%20apache%20status.png)

`COMMANDS TO CONFIGURE LOAD BALANCER: `

`sudo vi /etc/apache2/sites-available/000-default.conf`

`sudo systemctl restart apache2`

`sudo tail -f /var/log/httpd/access_log`

`sudo vi /etc/hosts`
`curl http://Web1`

![curl status](./Images/curl%20status.png)







