pipeline {
    agent {
        docker {
            image '3.9.8-sapmachine-11'
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

