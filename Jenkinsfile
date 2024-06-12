pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/SzyKOnar/jenkins-test-repo.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building the project..."'
               
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
                sh 'python3 -m unittest discover -s . -p "test_*.py"'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying the project..."'
            
            }
        }
    }
}