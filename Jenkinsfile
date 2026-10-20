pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Sharvil-14/Jenkins-Demo.git'
            }
        }

        stage('Build') {
            steps {
                bat '"C:\\Users\\Sharvil\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" app.py'
            }
        }

        stage('Test') {
            steps {
                bat '"C:\\Users\\Sharvil\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" test.py'
            }
        }
    }
}