pipeline {
    agent { docker { image 'node:20.11.1-alpine3.19' } }
    stages {
        stage('build') {
            steps {
                sh 'docker build -t hello-devops .'
                sh 'docker push us-east4-docker.pkg.dev/refined-magpie-418201/my-docker-repo/hello-devops'
            }
        }
    }
}