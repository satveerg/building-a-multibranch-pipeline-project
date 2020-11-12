pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                docker.image("centos:7").inside {
                    sh "echo hello"
                }
            }
        }
        
    }
}
