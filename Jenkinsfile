pipeline {
    agent any
    
    environment {
        DOCKER_REPO = "us-east4-docker.pkg.dev/refined-magpie-418201/my-docker-repo"
    }

    stages {
        stage("List env vars"){
			steps{
                sh "echo $DOCKER_REPO"
				sh "printenv | sort"
			}
		}


        stage('build') {
            steps {
                sh 'docker build -t $DOCKER_REPO${JOB_BASE_NAME}:{BUILD_ID} .'
                sh 'docker images'
                
                // sh 'docker tag '
                // sh 'docker push us-east4-docker.pkg.dev/refined-magpie-418201/my-docker-repo/hello-devops'
            }
        }
    }
}
