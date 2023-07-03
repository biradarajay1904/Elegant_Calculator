pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], userRemoteConfigs: [[url: 'https://github.com/biradarajay1904/Elegant_Calculator.git']]])
      }
    }

    stage('Build') {
      steps {
        bat 'fastlane build'
      }
    }
  }
}
