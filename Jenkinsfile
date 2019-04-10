pipeline {
    stages {
      stage('Test') {
        agent any
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
