pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'fastlane build'
            }
        }
        
        // Uncomment and add more stages for other lanes if needed
        /*
        stage('Beta') {
            steps {
                sh 'fastlane beta'
            }
        }
        
        stage('Deploy') {
            steps {
                sh 'fastlane deploy'
            }
        }
        */
    }
}
