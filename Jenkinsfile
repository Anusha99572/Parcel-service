pipeline {
  agent { label 'slave'}

  stages {
    stage ('checkout') {
      steps {
        sh 'rm -rf Parcel-service'
        sh "git clone https://github.com/Anusha99572/Parcel-service.git"
      }
    }
     stage ('build') {
      steps {
        sh '''
      sudo apt update
        '''
      }
    }
    stage ('deploy') {
      steps {
        sh '''
       pwd 
       ls
       '''
      }
    }
  }
  }
