pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Tanmay-Sherekar/App-python.git'
            }
        }

        stage('Install Python') {
            steps {
                sh 'python3 --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip3 install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'pytest'
            }
        }

        stage('Run Application') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
