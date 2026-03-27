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
        sh '''
        python3 -m venv venv
        . venv/bin/activate
        pip install -r requirements.txt
        '''
    }
}

        stage('Run Python App') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
