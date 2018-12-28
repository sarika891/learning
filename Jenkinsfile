node {
    checkout scm
}
pipeline {
    agent any
    environment {
        DISABLE_AUTH = 'true'
        DB_ENGINE = 'sqlite'
    }
    stages {
        stage('Build') {
            steps { 
                sh """
                wget ftp://ftp.csx.cam.ac.uk/pub/software/programming/pcre/pcre-8.42.tar.gz
                tar -zxf pcre-8.42.tar.gz
                cd pcre-8.42
                ./configure
                make
                make install	
                """
            }
        }
    }
}
