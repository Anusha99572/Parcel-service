pipeline {
  agent { lable 'slave'}

  stages {
    stage ('checkout') {
      steps {
        sh "git clone https://github.com/Anusha99572/Parcel-service.git"
      }
    }
     stage ('build') {
      steps {
        sh '''
        sudo apt update
        sudo apt install -y maven
        export JAVA_HOME=$(dirname $(dirname $(readlink -f $(which java))))
        export PATH=$JAVA_HOME/bin:$PATH
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
