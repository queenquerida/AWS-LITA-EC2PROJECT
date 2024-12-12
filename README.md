#AWS_LITA_PROJECT

Documentation process of launching an EC2 instance to host Apache web server for smartshop.
#### First step I did was create security group.
### Security Group Creation
created security group and set inbounds rules to allow HTTP and SSH traffic
image details below
![security group](/security_group.png)
#### Inbound Rules
inbound rules for the security Group created
![setting inbounds rules image](/inbound_rules.png)
#### Outbound Rules
the outbound rule was left at default to allow "all traffic"
![Outbound rules](/outbound_rule.png)
#### Image of successful Security Group created with details shown
![security group rules details](/Security_detail.png)
### Lauching of my EC2 instance
Launching of my EC2 instance details that would host the Apache web server
![EC2 Lauched](/ec2.png)
I Selected Amazon linux 2 as the OS and a t2.micro instance
![image of selected OS](/ami.png)
### Keypair was created
i created keypair and download it to my document
![image of successful keypair](/keyp.png)
####keypair was added to my EC2 instance
![keypair added](/key_pair.png)
### Added VPC under networks settings
I selected the already created vpc for this project image below.
![VPC](/lita_vpc.png)
#### Added subnet under the vpc
![public and privated subnet](/private_public.png)
#### public subnet selected 
![public subnet](/public_subnet.png)
### Added security group and set auto-assign the Public IP.
I added the security that i earlier created to the EC2 instance, also set the auto-assign public IP to enabled
![Security group to instance](/SG_A.png)
###Configure storage
I left the Configure storage at 8gb as advised
![Configure storage at 8gb](/config_storage.png)
### Finally Lauched my EC2 instance
image below showed that my EC2 instance has been launched and its initializing.
![Lauching EC2](/EC2_L.png)
#### Status check 
 status check below showed that my ec2 instance was ready to be connected
![status check 2/2](/ec2_status.png)
### Connecting my instance using the SSH client 
connected to the instance using the SSH client by coping the command"chmod 400"
![Connecting to instance](/connect_ssh.png)
### Deploying of the Apache web server 
I finally deploy the apache web server by installing it using code "sudo yum install httpd -y"
image below
![Apache Deployed](/apache_connected)
###Test Page
i copied the public Ip address on my EC2 instance and pasted it to the browser and i got the image below of my test Page
![Test page](/test_page.png)
