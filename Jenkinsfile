pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                    echo "hello world"
                    ./configure.sh
                    """
                }
            }
        }
    }
}
