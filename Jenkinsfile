pipeline {
    agent {
        docker {
            image '4.0.0'
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

