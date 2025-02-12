pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/kunalpuri123/CalculatorApp.git'
            }
        }
        
        stage('Clean') {
            steps {
                sh 'mvn clean'
            }
        }
        
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
