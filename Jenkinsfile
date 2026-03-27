pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Tanmay-Sherekar/App-python.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip3 install -r requirements.txt'
            }
        }

        stage('Run Python App') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
