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
                bat 'javac TimestampPrinter.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java TimestampPrinter'
            }
        }
    }
}
