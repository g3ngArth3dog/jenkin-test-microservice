pipeline{
	//agent any
	agent any
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
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