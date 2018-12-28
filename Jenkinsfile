node {
    checkout scm (1)
    
}
pipeline {
    agent any
    environment {
        DISABLE_AUTH = 'true'
        DB_ENGINE    = 'sqlite'
    }
    stages {
        stage('Build') {
            steps {
                sh "configure.sh"
				
            }
        }
    }
}
