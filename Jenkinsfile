pipeline {
    agent any
    stages {
        stage('Git Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Srivaishnavi08/week4'
            }
        }
        stage('Java Execution') {
            steps {
                bat '''
                javac week4.hello.java
                java week4.hello
                '''
            }
        }
        stage('Python Execution') {
            steps {
                bat 'python say.py'
            }
        }
    }
}
