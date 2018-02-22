pipeline { 
    agent any 
	def CC = 'clang'
	echo "lang is ${env.CC}	
    stages {
        stage('Build') { 
            steps { 
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
