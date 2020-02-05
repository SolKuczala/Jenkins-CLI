# Jenkins-CLI
briefly description of how to use it

Ensure to have X-SSH-Endpoint enabled

Inside a machine with jenkins running:

> curl http://192.168.18.232:8080//jnlpJars/jenkins-cli.jar

If you did not make a pair of KEYs

> ssh-keygen -t rsa

Go to webconsole and under "Configure Global security" enable security

Go to http://YOUR_JENKINS_HOSTNAME/user/USER/configuration and paste public key in "SSH public keys" 

Generate Token there in "API token" and copy it

Go to console where Jenkins is:

> java -jar jenkins-cli.jar -s http://JENKINS_HOST:PORT -auth USERNAME:TOKEN

Profit \o/

Available commands under http://YOUR_JENKINS_HOSTNAME/cli/
