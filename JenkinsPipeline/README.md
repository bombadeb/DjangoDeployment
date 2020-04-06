# Jenkins Pipeline script for CI job

Please find the steps for integration for the same.

## Jenkins installation on Centos 7
```bash
wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins.io/redhat-stable/jenkins.repo
rpm --import http://pkg.jenkins.io/redhat-stable/jenkins.io.key
yum install jenkins java-1.8.0-openjdk –y
systemctl start jenkins
systemctl enable jenkins
```

## Add the following in the sudoers file [sudo visudo -f /etc/sudoers]
```bash
jenkins ALL=(ALL) NOPASSWD: ALL
```

## Running the job 
```bash
Job Name : DjangoProjectBuildPipeline
Click --> Build with Parameter

Give the two parameters
1. DEVELOPMENT_BRANCH : master
2. DEPLOYMENT_BRANCH	: master 

Click --> Build
```
