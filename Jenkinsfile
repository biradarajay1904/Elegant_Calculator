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
                bat 'C:\\Ruby\\bin\\fastlane.bat build'
            }
        }
        
        // Uncomment and replace the bat commands for other stages if needed
        
        stage('Beta') {
            steps {
                bat 'C:\\Ruby\\bin\\fastlane.bat beta'
            }
        }
        
        stage('Deploy') {
            steps {
                bat 'C:\\Ruby\\bin\\fastlane.bat deploy'
            }
        }
    }
}
