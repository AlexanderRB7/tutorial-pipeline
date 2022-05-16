pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "hello world"
            }
        }
    }
    post {
        success {
            echo "Everything is fine."
            }
        failure {
            echo "Something is wrong."
        }
    }
}
