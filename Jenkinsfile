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
                javac HelloWorld.java
                java HelloWorld
                '''
            }
        }
        stage('Python Execution') {
            steps {
                bat 'python script.py'
            }
        }
    }
}
