pipeline {
	agent any
	triggers {
		pollSCM('* * * * *')
	}
	stages {
		stage('build'){
			steps {
				echo 'Build project'
			}
		}
		stage('test'){
			steps {
				echo 'Executing testes'
			}
		}
		stage('deployement'){
			steps {
				echo 'Deploying on target'
			}
		}
	}
	post {
		always {
			echo 'always'
		}
		success{
			echo 'success'
		}
	}
}
