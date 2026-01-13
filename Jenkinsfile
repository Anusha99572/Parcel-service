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
      whoami
      pwd
      ls
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
