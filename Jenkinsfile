pipeline {
    agent any
    stages {
        stage("List env vars"){
			steps{
				sh "printenv | sort"
			}
		}

        
        stage('build') {
            steps {
                sh 'docker build -t hello-devops .'
                sh 'docker images'
                sh 'echo ${env.WORKSPACE}'
                // sh 'docker tag '
                // sh 'docker push us-east4-docker.pkg.dev/refined-magpie-418201/my-docker-repo/hello-devops'
            }
        }
    }
}
