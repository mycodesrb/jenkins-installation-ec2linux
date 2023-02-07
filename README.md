# jenkins-installation-ec2linux
steps to install jenkins on EC2 instance

Open inbound port on EC2

[ec2-user ~]$ sudo yum update –y

[ec2-user ~]$ sudo wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo
    
[ec2-user ~]$ sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key

[ec2-user ~]$ sudo amazon-linux-extras install java-openjdk11 -y

[ec2-user ~]$ sudo yum install jenkins -y

[ec2-user ~]$ sudo systemctl enable jenkins

[ec2-user ~]$ sudo systemctl enable jenkins

[ec2-user ~]$ sudo systemctl status jenkins

hit publicip:8080
Initial PAssword page appears

do,
cat /var/lib/jenkins/secrets/initialAdminPassword
copy the long password and paste it there

jenkins starts..proceed
