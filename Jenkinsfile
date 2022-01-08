pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Completed...'
                timeout(time: 5, unit: 'SECONDS') {
                  sh 'sleep 10'
              }
            }
         }
        stage('test') {
            steps {
                echo 'Testing Completed...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Depolying Completed...'
            }
        }
    }
}