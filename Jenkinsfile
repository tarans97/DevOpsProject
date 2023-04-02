pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'  
                checkout scm
            }
        }

        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'  
                sh 'echo "Building..."'
                sh 'chmod 777 groupone.html'
                sh './groupone.html'
                
            }
        }

        stage('Test') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'  
                sh 'echo "Testing..."'
            }
        }

        stage('Deploy') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'  
                sh 'echo "Deploying..."'
            }
        }

       
    }
}
