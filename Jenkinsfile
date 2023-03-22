pipeline {
    agent any
    environment {
        BRANCH_NAME = "${env.BRANCH_NAME}"
    }
    stages {
        stage('checkout') {
            steps {
                git branch: 'main', credentialsId: '1', url: 'https://github.com/aditya10mm/nodejs-multibranch.git'
            }
        }
        stage('main Branch') {
            when {
                branch 'main'
            }
            steps {
                sh 'echo "Test branch dd. commit made!"'
            }
        }
        stage('dev Branch') {
            when {
                branch 'dev'
            }
            steps {
                sh 'echo "Main branch commit made! hurrryyyyyaaaaaaaa"'
            }
        }
    }
}
