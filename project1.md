# PROJECT 1
## LAMP STACK IMPLEMENTATION

**STEP1: APACHE INSTALLATION** 


1. Update packages from package manager

`sudo apt update`



![](images/1.png)






2. Run apache2 package installation

`sudo apt install apache2`




![](images/2.png)





3. Verify Apache2 services are running

`sudo systemctl status apache2`



![](images/4.png)



4. add a rule to EC2 configuration to open inbound connection through port 80


![](images/ec2rules.png)


5. Access server locally via DNS

`curl http://localhost:80`



![](images/5.png)



6. Retrieve your Public IP address locally

`curl -s http://169.254.169.254/latest/meta-data/public-ipv4`




![](images/6.png)


7. Test Apache HTTP server 
using http://<Public-IP-Address>:80
http://<http://35.173.220.234/>:80



![](images/7.png)






**STEP2: MYSQL INSTALLATION**

1. To acquire and install MYSQL 

`sudo apt install mysql-server`



![](images/8.png)

2. Run secure script

`sudo mysql_secure_installation`



![](images/9.png)


3. Configure password

![](images/10.png)


4. Test MYSQL

`sudo mysql`

![](images/sudomysql.png)




**STEP 3: PHP INSTALLATION**

1. Install PHP packages

`sudo apt install php libapache2-mod-php php-mysql`


![](images/11.png)


2. Confirm PHP version

`php -v`


![](images/12.png)

