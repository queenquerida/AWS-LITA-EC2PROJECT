#AWS_LITA_PROJECT

Documentation process of launching an EC2 instance to host Apache web server 
#### First step I did was create security group.
### Security Group Creation
created security group and set inbounds rules to allow HTTP and SSH traffic
image details below
![security group](/security_group.png)
inbound rules for the security Group created
![setting inbounds rules image](/inbound_rules.png)
#### Image of successful Security Group created with details shown
![security group rules details](/Security_detail.png)
### Lauching of EC2 instance
lauched EC2 instance details that would host the Apache web server
![EC2 Lauched](/ec2.png)
I Selected Amazon linux 2 as the OS and a t2.micro instance
![image of selected OS](/ami.png)
### Keypair was created
i created keypair and download it to my document
![image of successful keypair](/keyp.png)
####keypair was added to the EC2 instance
![keypair added](/key_pair.png)
### Adding Subnet
I selected the already created subnet for this project.
![public and privated subnet](/private_public.png)
#### public subnet selected
![public subnet](/public_subnet.png)
### Added security group
![Security group to instance](/SG_A.png)



