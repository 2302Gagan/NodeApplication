pipeline {
    agent {
        docker {
            image 'node:16' 
            args '-p 8080:8080' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                 git 'https://github.com/2302Gagan/NodeApplication.git'
                 bat 'node main.js' 
            }
        }
    }
}
