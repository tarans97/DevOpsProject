pipeline {
           agent {
        docker {
            image 'jenkins/jenkins:lts'
            args '-u root'
        } 
           
        }
           stages {
        stage('Build') {
           steps {
             git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'
                 sh './hello.sh'
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
