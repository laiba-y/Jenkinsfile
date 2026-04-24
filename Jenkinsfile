pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo Building...'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Testing...'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploying...'
            }
        }
    }
}
    post {
        always {
            echo 'This runs always'
        }
        success {
            echo 'Build was successful'
        }
        failure {
            echo 'Build failed'
        }
    }
}
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
