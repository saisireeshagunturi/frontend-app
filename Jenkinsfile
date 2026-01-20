pipeline {
  agent any

  environment {
    AWS_DEFAULT_REGION = 'us-east-1'
    S3_BUCKET = 'aws-s3-bucket-20260120'
    CLOUDFRONT_DISTRIBUTION_ID = ''
  }
  
  stages {
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }

    stage('Build frontend') {
      steps {
        sh 'echo "Static frontend build completed"'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy to S3 + CloudFront'
      }
    }
  }
}
