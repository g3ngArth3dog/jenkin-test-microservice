pipeline{
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