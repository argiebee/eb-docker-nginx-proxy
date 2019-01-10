pipeline {

    environment {

        BUILD_HOME='/var/lib/jenkins/workspace'

    }

    agent any

    stages {

        stage('checkout') {
            steps {
			    sh 'rm *.zip'
			    sh 'pwd'
			    sh 'ls'
			    checkout scm
				sh 'ls'
			}

        }

        stage('zip') {

            steps {
                zip zipFile:'eb-docker-nginx-proxy.zip', dir:'.'
				sh 'pwd'
				sh 'ls'
            }

        }

    }

}