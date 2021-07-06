# Devops
create an automation using Terraform:

First of all create a User on AWS and Generate Access and Secret Key.

Create a ec2.tf  and add the terraform code to it then export the AWS Access and Secret Keys then run 

terraform plan

terraform apply

After running the command , I can check the results using the show command or from the portal.

terraform.exe show 

Install the docker on Ubuntu VM:

 sudo apt-get update
 sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
	
	 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
	 
	 
	 Install Docker:
	 
	 sudo apt-get update
 sudo apt-get install docker-ce docker-ce-cli containerd.io

create a Dockerfile of a nginx containe

create a ngnix-docker file on ubuntu vm and paste the code then we have to build the image using below command:


docker build -t nginx-docker .

Then run the docker container on port 80

docker run -d -p 80:80 nginx-docker

Check the docker status by running the command docker ps -a


Install Jenkis on Linux VM:

sudo apt update
sudo apt install openjdk-8-jdk
wget –q –O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add –

sudo nano /etc/apt/sources.list

##Add below line:

#  Jenkins software repository
deb https://pkg.jenkins.io/debian binary

sudo apt install Jenkins

sudo systemctl status jenkins
