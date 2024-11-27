pipeline {
    agent any
    environment {
        PATH = "C:/Windows/System32
"
    }
    stages {
        stage('Git Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Srivaishnavi08/week4'
            }
        }
        stage('Java Execution') {
            steps {
               bat 'javac hello.java'
                bat 'java hello'
            }
        }
        stage('python Execution') {
            steps {
               bat 'python say.py'
            }
        }
    }
}
