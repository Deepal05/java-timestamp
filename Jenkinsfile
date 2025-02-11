pipeline {
    agent any
    triggers {
        githubPush()
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Deepal05/java-timestamp.git'
            }
        }
        stage('Build') {
            steps {
                sh 'javac Timestamp.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java Timestamp'
            }
        }
    }
}
