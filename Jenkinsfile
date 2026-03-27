pipeline {
  agent any

  stages {
    stage('clone repository'){
      steps {
        git 'https://github.com/Tanmay-Sherekar/App-python.git'
      }
    }

    stage('Build'){
      steps {
        sh 'echo "Build successful"'
      }
    }
  }
}
