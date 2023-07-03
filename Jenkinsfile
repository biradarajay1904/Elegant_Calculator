pipeline {
    agent any
    
    stages {
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
