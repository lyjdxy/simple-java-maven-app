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
	    	sh 'ping repo.maven.apache.org'
                sh 'mvn -B -X -DskipTests clean package'
            }
        }
    }
}
