:red_square: __Jenkins installation in Ubuntu__

:small_blue_diamond: update the server
```
# apt update -y
```
install java package
```
# apt install openjdk-11-jdk
```
```
# curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null
```
```
# echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null
```
update the repo
```
# apt-get update
```
install jenkins package
```
# apt-get install jenkins
```
start , enable and check status
```
# systemctl start jenkins
# systemctl enable jenkins
# systemctl status jenkins
```
check the ip address
```
# hostname -I
xx.xx.xx.xx
```
where xx.xx.xx.xx is the jenkins server ip

in browser
\
http://xx.xx.xx.xx:8080

find the default password for jenkins server
```
# cat /var/lib/jenkins/secrets/initialAdminPassword
```


