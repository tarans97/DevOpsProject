pipeline {
    agent {
        docker {
            image 'docker'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'
            }
        }
        stage('Build image') {
            steps {
                sh 'docker build -t myapp .'
            }
        }
        stage('Run container') {
            steps {
                sh 'docker run -p 80:80 -d myapp'
            }
        }
    }
}

