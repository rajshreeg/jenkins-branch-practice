
pipeline {
    agent any

    stages {
        stage('Checkout Information') {
            steps {
                echo 'Jenkins is connected to GitHub'
                echo 'Building the feature/login-demo branch'
                sh 'git --version'
                sh 'pwd'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage completed'
            }
        }
         stage('Developer Change') {
            steps {
                echo 'A developer pushed a change to develop'
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
