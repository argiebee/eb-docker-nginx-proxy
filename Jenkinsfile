pipeline {

    environment {

        BUILD_HOME='/var/lib/jenkins/workspace'

    }

    agent any

    stages {

        stage('checkout') {
            steps {
			    pwd
			    ls
			    checkout scm
				ls
			}

        }

        stage('zip') {

            steps {
                zip zipFile: 'eb-docker-nginx-proxy.zip', dir:'.'
				pwd
				ls
            }

        }

    }

}