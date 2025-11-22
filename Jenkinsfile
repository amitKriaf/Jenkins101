pipeline {
    agent {
        docker {
            image 'python:3.10'
        }
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Run HelloWorld') {
            steps {
                sh 'python python/helloworld.py'
            }
        }
    }
}
