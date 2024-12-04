ps aux | grep java

sudo tail -n 50 /var/log/jenkins/jenkins.log

journalctl -u jenkins.service --since "10 minutes ago"

tail -f /var/log/jenkins/jenkins.log

cat /var/lib/jenkins/secrets/initialAdminPassword

sudo usermod -aG docker jenkins

sudo passwd jenkins

sudo systemctl restart jenkins