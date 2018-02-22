pipeline { 
    agent any 	
    stages {
        stage('Build') { 
            steps { 
		checkout scm
		build 'demo'  
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
        stage('Test'){
            steps {
      		 echo "Test phase.."     
		}
        }
        stage('Deploy') {
            steps {
                echo "Deploy phase.."
            }
        }
    }
}
