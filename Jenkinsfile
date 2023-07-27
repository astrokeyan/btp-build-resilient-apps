pipeline {
  agent {
    node {
      label 'test'
    }

  }
  stages {
    stage('') {
      steps {
        sh '''cd /tmp
git clone https://github.com/astrokeyan/btp-build-resilient-apps btpapps
cd btpapps
npm run test
npm i -g typescript ts-node && npm install
npm run test
npm run build:cf'''
      }
    }

  }
}