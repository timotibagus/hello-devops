pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'docker build -t hello-devops .'
                sh 'docker images'
                sh 'docker push us-east4-docker.pkg.dev/refined-magpie-418201/my-docker-repo/hello-devops'
            }
        }
    }
}
