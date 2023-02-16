pipeline {
	agent any
	stages {
		stage('Build') { 
		steps {
			sh 'mvn clean install'
			echo 'Build stage Successful'
		}

	} 
	stage('Test') {
		steps {
		sh 'mvn test'
		echo 'Test Stage Successful'
		}
	} 
	stage('Deploy') { 
		steps {
			sh 'mvn deploy'
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
