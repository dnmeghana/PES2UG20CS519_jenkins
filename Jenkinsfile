pipeline {
	agent any
	stages {
		stage('Build') { 
		steps {
			echo 'Build stage Successful'
		}

	} 
	stage('Test') {
		steps {
		echo 'Test Stage Successful'
		}
	} 
	stage('Deploy') { 
		steps {
			echo 'Deployment Successful'
			}
		}
	}
	post { 
		failure { 
			echo 'Pipeline failed'
			 }
	}
}
