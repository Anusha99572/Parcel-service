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
     
     export JAVA_HOME=$(dirname $(dirname $(readlink -f $(which java))))
     export PATH=$JAVA_HOME/bin:$PATH
        '''
      }
    }
    stage ('deploy') {
      steps {
        sh '''
       mvn clean install
       mvn spring-boot:run
       '''
      }
    }
  }
  }
