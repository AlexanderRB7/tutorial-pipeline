pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
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
