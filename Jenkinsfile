pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/twoje-repozytorium.git', credentialsId: 'twoje-poświadczenia'
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
