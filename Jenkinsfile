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
                sh 'echo "Test branch dd. kjgkjkjg ii commdddit made!"'
                sh 'pwd'
                sh 'ls'
                sh 'scp -r $(pwd) . jenkins@3.110.119.76:/opt'
              
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
