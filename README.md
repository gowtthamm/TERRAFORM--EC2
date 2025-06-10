AUTOMATED DEPLOYMENT OF AN EC2 INSTANCE THROUGH TERRAFORM 

 <img src="https://github.com/gowtthamm/Terraform-EC2/blob/228fcf4d198ca6ae9f08b2c5c780b3d5029b60e6/Flowchart.png" >

 CONFIGURE TERRAFORM WITH AWS :
    aws configure 
    -->  Access Key ID : ************** 
    -->  Secret access Key : *******************
    -->  Region : ap-south-01 (Mumbai)
    -->   Output format : json

<img src="https://github.com/gowtthamm/Terraform-EC2/blob/d0c07a81368113b043e2fc6c126459adaac00903/AWS%20Configure.png" width="700" height="300">

		
 COMMANDS :
  01. terraform init 
           --> Initializes a Terraform Working Directory by Downloading required provider plugins and setting up the backend .
  02. terraform plan 
           -->  Terraform will make to your infrastructure without applying them , Helping ypu review before deployment .
  03. terraform apply 
           --> Execute the action proposed in the plan to create , update or delete infrastructure resource .
  
