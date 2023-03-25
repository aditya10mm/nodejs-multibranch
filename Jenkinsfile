pipeline {
    agent any
    environment {
        BRANCH_NAME = "${env.BRANCH_NAME}"
    }
    stages {
       
        stage('main Branch') {
            when {
                branch 'main'
            }
            steps {
                sh 'echo "Test branch dd. kjgkjkjg commdddit made!"'
            }
        }
        stage('dev Branch') {
            when {
                branch 'dev'
            }
            steps {
                sh 'echo "Main branch commit made! jhvaishbcij hurrryyyyyaaaaaaaa"'
            }
        }
    }
}
