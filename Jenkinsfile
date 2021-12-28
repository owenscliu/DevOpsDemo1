pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'BUILD is done'
      }
    }

    stage('Test') {
      steps {
        echo 'Test is done'
      }
    }

    stage('Notify') {
      steps {
        mail(subject: 'JENKINS NOTI', body: 'Jenkins is executed', to: 'owenliu@hkpc.org')
      }
    }

  }
  environment {
    BUILD_ID = 'BUILD_NUMBER'
  }
}