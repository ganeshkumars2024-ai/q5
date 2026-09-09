pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/ganeshkumars2024-ai/q5.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\HP\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" -m pip install -r requirement.txt'
            }
        }

        stage('Run Unit Tests') {
            steps {
                bat '"C:\\Users\\HP\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" -m pytest test_app.py -v'
            }
        }
    }
}