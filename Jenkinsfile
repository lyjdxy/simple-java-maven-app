pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
        }
    }
    stages {
        stage('Build') {
            steps {
	    	sh 'mvn -v'
	    	sh 'ping -c 4 199.232.192.215'
            }
        }
    }
}
