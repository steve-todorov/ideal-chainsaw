@Library('jenkins-shared-libraries') _

pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                withCredentials([usernameColonPassword(credentialsId: 'test_credentials', variable: 'TEST')]) {
                    sh "echo $TEST"
                }
            }
        }
    }
}
