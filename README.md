# Installation Jenkins Server


![Playbook Jenkins](https://cdn.ttgtmedia.com/visuals/LeMagIT/hero_article/Logo-Jenkins.jpg)

## Requirements

* install git
* install ansible

Go to the to clone the repository [Installation jenkins](https://github.com/AbdoulRahimBarry/Installation-Jenkins.git)

Run the ansible command

```
cd Installation-Jenkins
ansible-galaxy install -r requirements.yml
ansible-playbook jenkins_playbook.yml
```
* Add user docker and jenkins
```
sudo usermod -aG docker centos
sudo usermod -aG docker jenkins
```
Give privilege to jenkins to execute commands without password
```
sudo echo 'jenkins ALL=(ALL) NOPASSWD: ALL' >> /etc/sudoers
```

Connect to the jenkins server `http://@IP:8080`
