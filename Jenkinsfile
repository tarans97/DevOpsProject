pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'
            }
        }
        stage('Build') {
            steps {
                git 'https://github.com/tarans97/DevOpsProject.git'
              //  sh 'your build command here'
                echo "Build"
            }
        }
        stage('Test') {
            steps {
                git 'https://github.com/tarans97/DevOpsProject.git'
               // sh 'your test command here'
                echo "Test"
            }
        }
        stage('Deploy') {
            steps {
                git 'https://github.com/tarans97/DevOpsProject.git'
               // sh 'your deploy command here'
                echo "Deploy"
            }
        }
    }
}
