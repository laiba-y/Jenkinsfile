pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo Building...'
            }
        }

        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                bat 'echo Deploying on main branch'
            }
        }
    }
}
