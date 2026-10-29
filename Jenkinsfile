pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Verify Code') {
            steps {
                sh 'cat app.txt'
            }
        }

        stage('Test') {
            steps {
                sh 'test -s missing.txt'
                echo 'Test passed'
            }
        }
    }
}
