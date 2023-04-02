pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/tarans97/DevOpsProject.git'
            }
        }
        stage('Build') {
            steps {
                git 'https://github.com/tarans97/DevOpsProject.git'
              //  sh 'your build command here'
            }
        }
        stage('Test') {
            steps {
                git 'https://github.com/tarans97/DevOpsProject.git'
               // sh 'your test command here'
            }
        }
        stage('Deploy') {
            steps {
                git 'https://github.com/tarans97/DevOpsProject.git'
               // sh 'your deploy command here'
            }
        }
    }
}
