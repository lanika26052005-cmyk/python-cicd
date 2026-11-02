pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                sh '''
                    python3 -m venv venv
                    venv/bin/pip install -r requirements.txt
                '''
            }
        }

        stage('Run Tests') {
            steps {
                sh '''
                    venv/bin/python -m pytest -v
                '''
            }
        }

        stage('Build Docker Image') {
            steps {
                sh '''
                    docker build -t python-cicd:v1 .
                '''
            }
        }
    }
}
