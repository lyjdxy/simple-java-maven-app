pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
	    	sh 'mvn -v'
	    	sh 'which maven'
	    	sh 'which mvn'
	    	sh 'ping repo.maven.apache.org'
                sh 'mvn -B -X -DskipTests clean package'
            }
        }
    }
}
