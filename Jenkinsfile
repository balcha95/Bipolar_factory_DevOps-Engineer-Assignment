pipeline {
    agent { label 'slave2' }
	
    tools {
        // Install the Maven version configured as "M3" and add it to the path.
	        maven "maven"
    }

    stages { 
        stage('SCM Checkout') {
            steps {
                // Get some code from a GitHub repository
                 git 'https://github.com/balcha95/Bipolar_factory_DevOps-Engineer-Assignment.git'
            }
		}
        stage('Maven Build') {
            steps {
                // Run Maven on a Unix agent.
                sh "mvn -Dmaven.test.failure.ignore=true clean package"
            }
		}
	}
}
