
# AWS security group
  We are going to SSH from instance A to instance B and Instance B to instance A. instance A have SG-1 and instance B have SG-2
  ![sg](https://user-images.githubusercontent.com/59732833/182826586-b1ebd1bb-6801-4910-9920-9d7977e0ee7f.png)


## Step 1 
  Spin up 2 instance and attach default security group which have port 22 OPEN. if you have no idea how to launch new instance you can follow this link.
  https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-launch-instance-wizard.html
  
    
## Step 2 
   Create a 2 more security group with name SG-1 and SG-2
   ![image](https://user-images.githubusercontent.com/59732833/182826931-67987f27-6337-4694-9f63-01ba79307e59.png)

   Go to edit inbound rule for SG-1 and add SG-2 like in below pics

![image](https://user-images.githubusercontent.com/59732833/182826973-e0d14a6e-7013-48b1-b2f2-83b0e6068d19.png)

   Similer do the same step with SG-2 and add SG-1 there.
   
   
 ## step 3
  Go back to Ec2 instance and follow the below steps.
 ![image](https://user-images.githubusercontent.com/59732833/182827120-03d311d0-ae59-45f9-bb32-983de2dc34b2.png)
 
 ## step 4
  When you clik on change security group new page will open .Add SG-1 and save it. Do the 
  same step with instance 2
  ![image](https://user-images.githubusercontent.com/59732833/182827238-4997be1a-bfae-4e30-8008-e7f158eebf32.png)


## step 5
  connect your instance and ping using private IP with below command and you will see the result.
  -- ** ping 172.31.92.56
  
  ![Screenshot (598)](https://user-images.githubusercontent.com/59732833/182827560-e09d0bf8-2ef3-4405-95e9-0e3010f6ef6b.png)

  
   
