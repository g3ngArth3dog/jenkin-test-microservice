pipeline{
	//agent any
	agent { docker {
		image 'maven:3.6.3'
		}
	}
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				echo "Build tapos"
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