pipeline {
    //agent any	
	agent {
		docker {
			image 'maven:3.6.3'

		}
	}
		stages {
		    stage('Build') {
			    steps {
					sh "mvn --veriosn"
					echo 'build'
				}	
		}
			stage('Test') {
			    steps {
					echo "Test"
				}	
		}
		    stage('Integration Test')
			{
			    steps {
					echo "Integration Test"
				}	
		}
		
	} 
	post {
		always {
			echo 'I ran always'
		}
		success {
			echo 'I ran when successfull #2'
		}
		failure {
			echo 'I ran when fails!'
		}
	}
}
