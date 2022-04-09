pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
             agent {
                docker {
                    image 'python:2-alpine'
                }
            }
            steps {
                echo 'Testing..'
                sh 'python'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
