AUTOMATED DEPLOYMENT OF AN EC2 INSTANCE THROUGH TERRAFORM 

<img src="https://github.com/gowtthamm/Terraform-EC2/blob/228fcf4d198ca6ae9f08b2c5c780b3d5029b60e6/Flowchart.png" >

 CONFIGURE TERRAFORM WITH AWS :
<pre>
<code>
 aws configure 

    Access Key ID : 
    
    Secret access Key : 
    
    Region : ap-south-01 
    
    Output format : json
</code>
</pre>
 


 JSON CODE FOR EC2 DEPLOYMENT : 

    provider "aws" {
    region = "ap-south-1"
    }

    resource "aws_instance" "redhat1" {
    ami           = "ami-0f535a71b34f2d44a"
    instance_type = "t2.micro"
    tags = {
    Name = "RedHat-EC2-1"
     }
    }

 

<img src="https://github.com/gowtthamm/Terraform-EC2/blob/d0c07a81368113b043e2fc6c126459adaac00903/AWS%20Configure.png" width="600" height="300">

		
 TERRAFORM COMMANDS :
 <pre>
<code>
terraform init 

terraform plan 
        
terraform apply 

terraform destroy
</code>
</pre>
       

--> INIT : Initializes a Terraform Working Directory by Downloading required provider plugins and setting up the backend

--> PLAN : Terraform will make to your infrastructure without applying them , Helping ypu review before deployment 

--> APPLY: Execute the action proposed in the plan to create , update or delete infrastructure resource

--> DESTROY : Delete all resources managed by the current terraform configuration .



<img src="https://github.com/gowtthamm/Terraform-EC2/blob/bf20f7b631f3d42d79c3d70e0b295a9ad68874f2/Apply.png" width="600" height="300">

<img src="https://github.com/gowtthamm/Terraform-EC2/blob/bf20f7b631f3d42d79c3d70e0b295a9ad68874f2/Deployed.png" width="600" height="300">

DESTROYED :

<img src="https://github.com/gowtthamm/Terraform-EC2/blob/bf20f7b631f3d42d79c3d70e0b295a9ad68874f2/Destory.png">

<img src="https://github.com/gowtthamm/Terraform-EC2/blob/bf20f7b631f3d42d79c3d70e0b295a9ad68874f2/Destroyed.png" >

