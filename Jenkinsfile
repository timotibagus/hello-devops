pipeline {
    agent { docker { image 'node:20.11.1-alpine3.19' } }
    stages {
        stage('build') {
            steps {
                sh 'docker build -t hello-devops .'
                sh 'docker run -d hello-devops'
                sh 'Deploy Completed'
            }
        }
    }
}