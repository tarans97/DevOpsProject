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

        stage('Install Docker') {
            steps {
                script {
                    def dockerInstalled = sh(script: 'which docker', returnStatus: true) == 0

                    if (!dockerInstalled) {
                        sh 'curl -fsSL https://get.docker.com -o get-docker.sh'
                        sh 'sudo chmod +x get-docker.sh'
                        sh './get-docker.sh'
                        sh 'sudo usermod -aG docker taranvir'
                    } else {
                        echo 'Docker is already installed.'
                    }
                }
            }
        }
    }
}
