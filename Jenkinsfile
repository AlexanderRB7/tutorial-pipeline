pipeline {
    agent { docker { image 'maven:3.8.4-openjdk-11-slim' } }
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
