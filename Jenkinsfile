pipeline {
    agent none
    stages {
      stage('Test') {
        steps {
          sh('printenv')
        }
      }
      stage('Docker') {
        agent {
          docker { image 'node:7-alpine' }
        }
        steps {
          sh 'node --version'
        }
      }
    }
}
