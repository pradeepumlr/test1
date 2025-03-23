pipeline {
    agent any
    stages {
        stage('Deploy with Ansible') {
            steps {
                sh 'ansible-playbook -i hosts.ini deploy_app.yml'
            }
        }
    }
}
