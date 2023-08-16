pipeline {
    agent {
        node {
            label 'docker-agent-python'
        }
    }

    triggers {
        pollSCM 'H/2 * * * *'
    }

    stages {
        stage('Build') {
            steps {
                echo "Building..."
                sh '''
                echo "doing build stuff here..."
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing..."
                sh '''
                echo "doing testing stuff here..."
                '''
            }
        }
        stage('Deliver'){
            steps {
                echo "Deliver..."
                sh '''
                echo "doing deployment here..."
                '''
            }
        }
    }
}