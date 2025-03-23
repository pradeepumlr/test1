pipeline { 
    agent any 
    stages { 
        stage('Build') { 
            steps { 
                bat 'mvn clean package'  // Use 'bat' instead of 'sh' for Windows
            } 
        } 
    } 
}
