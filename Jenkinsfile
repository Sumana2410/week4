pipeline {
    agent any
    stages {
        stage('Git Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/your-username/your-repo.git'
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
