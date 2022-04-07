pipeline{
	agent any
	//agent {
	//	docker {
	//		image 'python:alpine3.10'
	//	}
	//}
	stages {
		stage('Build') {
			steps {
				sh 'python --version'
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration test') {
			steps {
				echo "Integration test"
			}
		}
	} 

	post {
		always {
			echo 'running'
		}
		success {
			echo 'success'
		}
		failure {
			echo 'failed'
		}
	}
}