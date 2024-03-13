 1  sudo apt update
    2  sudo apt install openjdk-11-jre
    3  java -version
    4  sudo wget -O /usr/share/keyrings/jenkins-keyring.asc   https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
    5  echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]   https://pkg.jenkins.io/debian-stable binary/ | sudo tee   /etc/apt/sources.list.d/jenkins.list > /dev/null
    6  sudo apt-get update
    7  sudo apt-get install jenkins
    8  history
    9  jenkins
   10  ps -ef | grep jenkins
   11  clear
   12  cat /var/lib/jenkins/secrets/initialAdminPassword
   13  sudo cat /var/lib/jenkins/secrets/initialAdminPassword
   14  sudo apt install docker.io
   15  sudo su -
    1  usermod -aG docker jenkins
    2  usermod -aG docker ubuntu
    3  systemctl restart docker
    4  su - jenkins
