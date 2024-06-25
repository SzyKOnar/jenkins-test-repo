pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/SzyKOnar/jenkins-test-repo.git', credentialsId: 'twoje-poświadczenia'
            }
        }
        stage('Build') {
            steps {
                sh 'make build'
            }
        }
        stage('Test') {
            steps {
                sh 'make test' 
            }
        }
    }
}
//zmiana
