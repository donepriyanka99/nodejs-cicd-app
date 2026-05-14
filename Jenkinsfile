pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo 'Code Cloned'
            }
        }

        stage('Build') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'node app.js'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Application Deployed'
            }   
        }
    }

    post {
        success {
            echo 'Pipeline Success'
        }

        failure {
            echo 'Pipeline Failed'
            
        }
    }
}
