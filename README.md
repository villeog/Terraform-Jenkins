Jenkins Terraform Installation:

Take amazon-linux-2023 instance - 4 GB RAM

sudo yum install -y java-11-amazon-corretto

sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo

sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key

sudo yum install -y jenkins

sudo systemctl start jenkins

sudo yum-config-manager --add-repo https://rpm.releases.hashicorp.com/AmazonLinux/hashicorp.repo

sudo yum install yum-utils awscli unzip maven git tree terraform -y

sudo systemctl enable jenkins



