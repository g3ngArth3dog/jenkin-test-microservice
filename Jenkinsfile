pipeline{
	//agent any
	agent {
		docker {
			image 'maven:3.8.5-jdk-11'
		}
	}
	stages {
		stage('Build') {
			steps {
				//sh 'maven --version'
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
			echo 'test 1'
		}
		success {
			echo 'test 2'
		}
		failure {
			echo 'failed'
		}
	}
}