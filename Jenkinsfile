pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/tumpillipavan/Kavita.git'
            }
        }

        stage('Build') {
            steps {
                dir('MavenHelloWorld-main') {
                    sh 'mvn clean package'
                }
            }
        }

        stage('Test') {
            steps {
                dir('MavenHelloWorld-main') {
                    sh 'mvn test'
                }
            }
        }
    }
}
