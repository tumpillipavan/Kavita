pipeline {
    agent any

    tools {
        maven 'maven3'
    }

    stages {
        stage('Build') {
            steps {
                dir('Kavita') {
                    sh 'mvn clean package'
                }
            }
        }

        stage('Test') {
            steps {
                dir('Kavita') {
                    sh 'mvn test'
                }
            }
        }
    }
}
