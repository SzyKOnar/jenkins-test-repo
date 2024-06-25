pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/SzyKOnar/jenkins-test-repo.git', branch: 'main', credentialsId: 'twoje-poświadczenia'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Build stage"' 
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Test stage"' 
            }
        }
    }
}

//zmiana
