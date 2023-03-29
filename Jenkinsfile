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
                sh 'echo "Test branch ddd. kjgkjkjg ii commdddit made!"'
                sh 'pwd'
                sh 'ls'
                sh 'scp -r $(pwd) . jenkins@172.24.191.79:/home'
              
            }
        }
        stage('dev Branch') {
            when {
                branch 'dev'
            }
            steps {
                sh 'echo "Main branch commit made! jhvaishbcijfff hurrryyyyyaaaaaaaa"'
            }
        }
    }
}
