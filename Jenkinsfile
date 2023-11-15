pipeline {
	agent any
	
	stages {
		stage('Build') {
			steps {
				bat 'composer install'
			}
		}
		stage('Test') {
			steps {
                powershell './vendor/bin/phpunit tests'
            }
		}
	}
}