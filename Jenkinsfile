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
	    	sh 'ping 199.232.192.215'
		sh 'cat /etc/resolv.conf'
	    	sh 'ping repo.maven.apache.org'
                sh 'mvn -B -X -DskipTests clean package'
            }
        }
    }
}
