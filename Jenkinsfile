pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/pradeepumlr/test1'
            }
        }
        stage('Debug') {
            steps {
                // Print environment variables to check if mvn and git are available
                bat 'echo %PATH%'
                bat 'mvn -v'  // Check Maven version
                bat 'git --version'  // Check Git version
            }
        }
        stage('Build') {
            steps {
                // Run Maven build
                bat 'mvn clean package'
            }
        }
    }
}
