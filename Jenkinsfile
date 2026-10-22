
pipeline {
    agent any

    stages {
        stage('Checkout Information') {
            steps {
                echo 'Jenkins is connected to GitHub'
                echo 'Building the main branch'
                sh 'git --version'
                sh 'pwd'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage completed'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the console output.'
        }
    }
}
