pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/pradeepumlr/test1'
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
        stage('Deploy') {
            steps {
                bat 'ansible-playbook deploy.yml'
            }
        }
    }
}
