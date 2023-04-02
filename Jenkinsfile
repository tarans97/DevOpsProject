pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building..."'
                sh 'hello.sh'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Testing..."'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying..."'
            }
        }

       
    }
}
