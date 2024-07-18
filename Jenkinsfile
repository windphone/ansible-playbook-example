pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/windphone/ansible-playbook-example.git'
            }
        }
        
        stage('Run Ansible Playbook') {
            steps {
                ansiblePlaybook credentialsId: '', 
                                inventory: 'hosts', 
                                playbook: 'site.yml'
            }
        }
    }
}

