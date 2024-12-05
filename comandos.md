ps aux | grep java

sudo tail -n 50 /var/log/jenkins/jenkins.log

journalctl -u jenkins.service --since "10 minutes ago"

tail -f /var/log/jenkins/jenkins.log

sudo cat /var/lib/jenkins/secrets/initialAdminPassword

sudo usermod -aG docker jenkins

sudo passwd jenkins

sudo systemctl restart jenkins

Dentro do Jenkins
Baixar os plugins SonarQube Scanner e Pipeline: Stage View

![alt text](./images/sonar-server.png)

![alt text](./images/sonar-scanner.png)