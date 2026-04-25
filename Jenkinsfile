pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'declerative pipeline'
            }
        }
        stage('Test') {
            steps {
                sh 'test'
            }
        }
    }
    post {
        failure {
            mail to: 'team@company.com', subject: 'Build Failed'
        }
    }
}
