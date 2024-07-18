pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', 
                          branches: [[name: '*/main']],
                          userRemoteConfigs: [[url: 'https://github.com/windphone/ansible-playbook-example.git']]
                ])
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

