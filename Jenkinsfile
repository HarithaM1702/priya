pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: https://github.com/HarithaM1702/priya.git, branch: 'main'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to server...'
            }
        }
    }
}
