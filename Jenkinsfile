pipeline {
  agent any

  stages {
    stage('clone repository'){
      steps {
        git 'https://github.com/Tanmay-Sherekar/App-python.git'
      }
    }

    stage('Install dependencies') {
      steps {
        sh 'pip3 install -r requirements.txt'
      }
    }

    stage('Run Tests') {
      steps {
        sh 'pytest'
      }
    }

    stage('Build'){
      steps {
        sh 'echo "Build successful"'
      }
    }
  }
}
