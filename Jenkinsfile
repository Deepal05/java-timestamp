pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Deepal05/java-timestamp.git'
            }
        }
        stage('Build') {
            steps {
                sh 'javac TimestampPrinter.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java TimestampPrinter'
            }
        }
    }
}
