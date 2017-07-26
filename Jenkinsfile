pipeline {
  agent none
  stages {
    stage('upgrade') {
      steps {
        echo 'Upgrading..'
        sh 'ls'
      }
    }
    stage('') {
      steps {
        parallel(
          "test on 5FA0": {
            echo 'test on 5FA0'
            
          },
          "test on 5FA1": {
            echo 'test on 5FA1'
            
          },
          "test on 5FA2": {
            echo 'test on 5FA2'
            
          }
        )
      }
    }
    stage('Reporting') {
      steps {
        isUnix()
      }
    }
  }
}