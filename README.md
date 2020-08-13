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
Connect to the jenkins server `http://@IP:8080`
