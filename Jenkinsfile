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
        
        // Uncomment and add more stages for other lanes if needed
        
        /*
        stage('Beta') {
            steps {
                bat 'fastlane beta'
            }
        }
        
        stage('Deploy') {
            steps {
                bat 'fastlane deploy'
            }
        }
        */
    }
}
