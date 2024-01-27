Ansible,Jenkins, Docker & Terraform Installation:

Take amazon-linux-2 instance

yum update -y

sudo amazon-linux-extras install java-openjdk11 -y

sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo

sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io-2023.key

sudo yum-config-manager --add-repo https://rpm.releases.hashicorp.com/AmazonLinux/hashicorp.repo

sudo yum install yum-utils epel awscli unzip maven git tree docker jenkins terraform -y

sudo systemctl start docker

sudo systemctl enable docker

sudo systemctl start jenkins

sudo systemctl enable jenkins

