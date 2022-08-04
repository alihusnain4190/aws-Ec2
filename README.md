
# AWS security group
  We are going to SSH from instance A to instance B and Instance B to instance A. 
  ![sg](https://user-images.githubusercontent.com/59732833/182826586-b1ebd1bb-6801-4910-9920-9d7977e0ee7f.png)


## Step 1 
  Spin up 2 instance and attach default security group which have port 22 OPEN.
## Step 2 
   Create a 2 more security group with name SG-1 and SG-2
   
   Go to edit inbound rule for SG-1 and add SG-2 like in below pics
    
   Similer Go to edit inbound rule in SG-2 and add SG-1 there 
   
 ## step 3
  Go back to Ec2 instance and follow the below screen shot step
  
 ## step 4
  When you clik on change security group new page will open .Add SG-1 and save it. Do the 
  same step with instance 2
  
  
  
   
