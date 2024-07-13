pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    // Pull the Maven Docker image
                    docker.image('maven:3.8.4').pull()
                    
                    // Run Maven commands
                    docker.image('maven:3.8.4').inside {
                        sh 'mvn clean install'
                    }
                }
            }
        }
    }
}

