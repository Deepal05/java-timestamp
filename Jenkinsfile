pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Deepal05/java-timestamp.git'
            }
        }
        stage('Compile') {
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
