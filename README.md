## Overview of the Project ##
Check out the [presentation](https://docs.google.com/presentation/d/16TAjmNnzbAIgkA4dyEK4xFmHskRC4CN1ynMVLxDHuSc/edit?usp=sharing)!

1. Provision a Kubernetes environment using VirtualBox, Vagrant, and Ansible playbooks.
2. Create a Jenkins(CI/CD) pipeline to deploy the Flask application onto the Kubernetes cluster.
3. Monitor the application with Promthethus and Grafana
4. Create a load with a tool like stress to simulate application activity. 

![](https://i.imgur.com/13cMnq8.png)

## Provisioning a Kubernetes Cluster with Virtual Box, Vagrant, and Ansible playbooks ##

Following the documentation here [https://www.ansibleforkubernetes.com/](https://www.ansibleforkubernetes.com/)

1. Create and configure Vagrantfile to spin up two VMs. One Master node and one worker node.
![](https://i.imgur.com/UHmluFb.png)
 
2. Now I can SSH into any of the VMs using:
   `vagrant ssh kube1`
