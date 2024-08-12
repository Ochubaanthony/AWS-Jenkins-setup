Pre-requisites:
 at least memory should be t2.medium (4 GB RAM)
port 8080 opened in firewall rule to access Jenkins
Connect to EC2 instance using git bash or iTerm
cd Downloads
ssh -i jenkins.pem ubuntu@12345678
chmod 600 jenkins.pem
ssh -i jenkins.pem ubuntu@12345678

Change Host Name to Jenkins
sudo hostnamectl set-hostname Jenkins


Perform update first
sudo apt update

Install Java 17
sudo apt install openjdk-17-jdk -y


Verify Java Version
java -version

Maven Installation
Maven is a popular build tool used for building Java applications. Please click here to learn more about Maven. You can install Maven by executing below command:

sudo apt install maven -y

you can type mvn --version
you should see the below output.


Jenkins Setup

Add Repository key to the system
Append debian package repo address to the system
copy both  command code from jenkins home page 


Update Ubuntu package
sudo apt update


Install Jenkins
sudo apt install jenkins -y


Access Jenkins in web browser
ec2-18-444-333-298.eu-central-1.compute.amazonaws.com:8080


Get the initial password from the below file
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
copy the password from the terminal and paste on the browser

getting start by adding the details









