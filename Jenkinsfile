pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                docker.withRegistry('https://hub.docker.com/_/centos') {
                  docker.image('centos:7').inside {
                    sh "echo hello"
                }
            }
        }
        
    }
}
}
