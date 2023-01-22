# AWS-CloudFormation-Jenkins

## Installing Jenkins on your local or AWS Instance Ubuntu:

1. For updating your system if you are first time booting up
   - Sudo apt update
  
2. Install java because jenkins run on java
   - Sudo apt-install openjdk-11-jre
  
3. Install Jenkins
    - curl -fsSL https://pkg.jenkins.io/debian/jenkins.io.key | sudo tee \   /usr/share/keyrings/jenkins-keyring.asc > /dev/null 
    - echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \   https://pkg.jenkins.io/debian binary/ | sudo tee \ /etc/apt/sources.list.d/jenkins.list > /dev/null
    - Sudo apt-get update
    - Sudo apt-get install jenkins
    - Sudo systemctl enable jenkins
    - Sudo systemctl start jenkins
4. Open port 8080 from your ip in security  group because jenkins run on 8080
5. Open your jenkins hosted public ip address in your web browser 3.82.93.143:8080
6. Go to your ec2 terminal and type
      - Sudo cat /var/lib/jenkins/secrets/initialAdminPassword
7. Copy it and paste it in Jenkins and click on continue
8. CloudFormation and Jenkins integration
      - Install cloud formation plugin
      - Click on new item and build freestyle project
      - Give github repo url
      - Enter Cloud Formation varibale
      - Create IAm Role on AWS
      - Give access key and secret key in Jenkins configuration

  
  
 



 
 



   
