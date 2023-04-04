## Project Title - Deploy a high-availability web app using CloudFormation
This folder provides the starter code for the "ND9991 - C2- Infrastructure as Code - Deploy a high-availability web app using CloudFormation" project. 
You must execute the vpc_subnet.yml script first and only once completed you can execute lb_server.yml
I've splitted the vpc/subnet components form the alb/ec2 components to make the debuging easier
 
This folder contains the following files:

>### **vpc_subnet.yml**
>>This file contains all the information to set up the vpc, subnets, route tables and gateways.

>### **vpc_subnet_params.json**
>>File contains the parameter information for vpc_subnet.yml 

>### **lb_server.yml**
>>This file contains all the information to set up the ec2 Iam role, alb and ec2 security groups, alb details(target group, listnener, launch config ect.) and autoscaining details

>### **lb_server_params.json**
>>File contains the parameter information for lb_server.yml 

### <span style="color:red">NOTE :</span> ###
you must chnage the s3 folder location in **lb_server_yml** file line 99 before you run the script. If you dont have an s3 bucket and index file you can replace line 99 with:  <br /> echo "Udacity Demo Web Server Up and Running" > index.html