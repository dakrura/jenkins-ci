pipeline {
  agent {
    docker {
      image 'ubuntu'
      args 'latest'
    }
    
  }
  stages {
    stage('update') {
      steps {
        sh 'pwd'
        sh 'echo "12D2 64E3" > tap_lst.txt'
      }
    }
    stage('run tests') {
      steps {
        readFile 'tap_lst.txt'
        sh 'cat tap_lst.txt'
      }
    }
  }
}