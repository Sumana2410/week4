pipeline {
    agent any
    environment {
        PATH = "C:/Windows/System32;C:/Users/suman/AppData/Local/Programs/Python/Python312;C:/Program Files/Java/jdk-21/bin"
    }
    stages {
        stage('Git Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Sumana2410/pipeline.git'
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
