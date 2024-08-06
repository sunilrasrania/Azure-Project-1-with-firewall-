# Azure-Project-1-with-firewall-
Deploying an application behind Firewall on Azure 

this is our first project on azure 

**in this project we will deploy a application on azure with firewall and bastion**

## step-1 

first we create a virtual network 

in this virtual network we will create a firewall , behind this firewall we will setup a subnet (web application subnet) , we will enable azure bastion
in this web application subnet (defalt subnet), we will deploy a virtual machine. 

in this vm we will nginx , we will host a static html page.

**resource group**

create a resourse group 

**create a vnet**

1. create a virtual network
2. enable azure bastion
3. create a public add. (delete this after use)
4. enable azure firewall

**create vm**

keep in mind two things
1.we choose subnet (default one)
2.download ssh key file

after creation we don't have any public ip address to connect our vm to the terminal, 

in that time we use bastion connect 

**bastion**

this bastion provide us a proper iam policy that only certian user can access our vm or applicaiton

**for this bastion connect**

1. go to connect mode of vm
2. give name azure user
3. aunth. type- choose ssh private key form local file
4. click on connect

**with all of  this we can connect and we can host our application behind the firewall**
