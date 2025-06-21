pipeline {
    agent any

    stages {
        stage('Code Checkout') {
            steps {
                git 'https://github.com/Bile-git/IGP-may31.git'
            }
        }
    }
    stages {
        stage('Code Compile') {
            steps {
                sh 'mvn compile'
            }
        }
    }
    stages {
        stage('Unit Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
    stages {
        stage('Code packaging') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
