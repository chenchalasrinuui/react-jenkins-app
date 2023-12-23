pipeline {
  agent any

  stages {
    stage('Install Dependencies') {
      steps {
        script {
          sh 'npm install'
        }
      }
    }

    stage('Build') {
      steps {
        script {
          sh 'npm run build'
        }
      }
    }

    stage('Deploy to S3') {
      steps {
        script {
          sh 'aws s3 sync build/ s3://your-s3-bucket-name'
        }
      }
    }
  }
}
