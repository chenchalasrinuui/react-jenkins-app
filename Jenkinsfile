pipeline {
  agent any

  stages {
    stage('Install Dependencies') {
      steps {
        script {
          echo "sss"
          bat 'npm install'
        }
      }
    }

    stage('Build') {
      steps {
        script {
          bat 'npm run build'
        }
      }
    }
  }
}
