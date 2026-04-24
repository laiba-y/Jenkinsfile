pipeline {
    agent any

    parameters {
        string(name: 'USERNAME', defaultValue: 'User', description: 'Enter your name')
    }

    environment {
        NAME = "Laiba"
    }

    stages {
        stage('Build') {
            steps {
                bat 'echo Building...'
            }
        }

        stage('Test') {
            steps {
                bat "echo Hello %USERNAME%"
            }
        }

        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                bat 'echo Deploying...'
            }
        }
    }

    post {
        always {
            echo 'Always runs'
        }
        success {
            echo 'Success!'
        }
        failure {
            echo 'Failed!'
        }
    }
}
