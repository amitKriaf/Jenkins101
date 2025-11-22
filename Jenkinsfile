pipeline {
    agent {
        docker {
            image 'python:3.10-alpine'
        }
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Run Python Script') {
            steps {
                sh 'python3 helloworld.py'
            }
        }
    }
}
