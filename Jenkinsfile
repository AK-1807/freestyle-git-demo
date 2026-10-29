pipeline {
    agent any
    
    // Poll SCM trigger: polls every 2 minutes
    triggers {
        pollSCM('H/2 * * * *')
    }
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
                echo 'Checkout stage complete.'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to staging environment and checking pipeline automation'
            }
        }
    }
}
