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
                //sh './mvnw clean install site surefire-report:report'
               // sh 'tree'
                //sh 'chmod 777 hello.sh'
                //sh './hello.sh'
                //Testing
                 
                
                   // docker.build("my-nginx-image")
                   // docker.withRegistry('https://registry.example.com', 'docker-credentials') {
                     //   docker.image("my-nginx-image").push()
                    
                
                
            }
        }
        

        stage('Test') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'  
                sh 'echo "Testing..."'
                
                
                    //docker.run("my-nginx-container", "--name my-nginx-container -p 80:80 -d my-nginx-image")
                
            
        }

        stage('Deploy') {
            steps {
                git branch: 'main', url: 'https://github.com/tarans97/DevOpsProject.git'  
                sh 'echo "Deploying..."'
            }
        }
    }
    
    post {
        success {
            publishHTML([
                allowMissing: false,
                alwaysLinkToLastBuild: false,
                keepAll: false,
                reportDir: '',
                reportFiles: 'groupone.html',
                reportName: 'GroupOne Project Report',
                reportTitles: '',
                useWrapperFileDirectly: true
            ])
        }
    }
}
    }
