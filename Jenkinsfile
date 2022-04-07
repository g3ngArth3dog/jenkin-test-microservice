pipeline{
	//agent any
	agent {
		docker {
			image 'alphine/helm'
		}
	}
	stages {
		stage('Build') {
			steps {
				sh 'helm ls'
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