pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Tanmay-Sherekar/App-python.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Build successful"'
            }
        }
    }
}
