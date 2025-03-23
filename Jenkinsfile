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
    }
}
