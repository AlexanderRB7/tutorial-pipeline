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
        mail to: 'alexanderborroto@rccl.com',
             subject: "Working Pipeline",
             body: "Working as expected."
        }
    }
}
