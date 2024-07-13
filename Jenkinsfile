pipeline {
    agent {
        docker {
            image 'maven:3.3.1'
        }
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install -X'
            }
        }
    }
}

