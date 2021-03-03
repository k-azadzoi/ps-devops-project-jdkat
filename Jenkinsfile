pipeline {
    agent any

    stages {
        stage('Cloning git repo') {
            steps {
                sm 'rm -f ps-devops-project-jdkat'
                sh 'git clone https://github.com/k-charette/ps-devops-project-jdkat'
            }
        }
        stage('Execute Ansible'){
            steps {
                ansiblePlaybook disableHostKeyChecking: true, installation: 'ansible', inventory: 'inventory', playbook: 'test-deployment.yml'
            }
        }
    }
}