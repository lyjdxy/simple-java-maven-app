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
		# sh 'cat /etc/resolv.conf'
		# sh 'ls -l /usr/share/maven/'
		# sh 'cat /usr/share/maven/conf/settings.xml'
	    	# sh 'ping repo.maven.apache.org'
                # sh 'mvn -B -X -DskipTests clean package'
            }
        }
    }
}
