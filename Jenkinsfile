pipeline {
	agent any
	
	stages {
		stage('Build') {
			steps {
				powershell 'composer install'
			}
		}
		stage('Test') {
			steps {
                powershell './vendor/bin/phpunit tests'
            }
		}
	}
}