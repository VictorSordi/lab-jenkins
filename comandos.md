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



docker run -d -p 8091:8081 -p 8123:8123 --name nexus -v nexus-data:/nexus-data sonatype/nexus3

cat /nexus-data/admin.password 


cd /var/lib/jenkins/workspace/projeto

docker build -t  devops/app .

docker login localhost:8123

docker tag devops/app:latest localhost:8123/devops/app

docker push localhost:8123/devops/app