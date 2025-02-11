pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-username/java-timestamp.git'
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
