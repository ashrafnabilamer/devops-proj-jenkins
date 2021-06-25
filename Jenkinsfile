pipeline {
    agent any	
		stages {
		    stage('Build') {
			    steps {
					echo "Build"
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
			echo 'I ran when successfull'
		}
	}
}
