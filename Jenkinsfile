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
                sh 'npm install'
                sh 'npm run build'
              
                
            }
        }
         stage('Publish') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'  
                publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: true, reportDir: 'dist', reportFiles: 'groupone.html', reportName: 'GroupOne Project Report'])

              
                
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
