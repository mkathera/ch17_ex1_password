pipeline { 
    agent any 	
    stages {
        stage('Build') { 
            steps { 
		git url: 'https://github.com/mkathera/ch17_ex1_password.git'    
		env.PATH = "${tool 'Ant'}/bin:${env.PATH}"
  		sh 'ant build'  
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
