pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo Building...'
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
