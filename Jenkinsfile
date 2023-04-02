pipeline {
    agent any
    stages {
        
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'
            }
        }
        stage('Install Docker') {
    steps {
        sh 'curl -fsSL https://get.docker.com -o get-docker.sh'
        sh 'sh get-docker.sh'
    }
        stage('Build') {
            steps {
                
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'
              //  sh 'your build command here'
                sh 'docker --version'
                echo "Build"
            }
        }
        stage('Test') {
            steps {
              
              git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'  
               // sh 'your test command here'
                echo "Test"
            }
        }
        stage('Deploy') {
            steps {
                
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'
               // sh 'your deploy command here'
                echo "Deploy"
            }
        }
    }
}
