pipeline{
	agent any
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
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