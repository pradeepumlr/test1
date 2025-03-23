pipeline {
    agent any
    environment {
        PATH = "D:\\apache-maven-3.9.9\\bin;${env.PATH}"
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
        stage('Deploy with Ansible') {
            steps {
                bat '''
                cd C:\\ansible\\playbooks
                ansible-playbook -i hosts.ini deploy_app.yml -vvv
                '''
            }
        }
    }
}
