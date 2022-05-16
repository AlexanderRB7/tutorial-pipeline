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
    failure {
        mail to: 'alexanderborroto@rccl.com',
             subject: "Failed Pipeline",
             body: "Something is wrong"
        }
    }
}
