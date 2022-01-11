pipeline {
    agent any

    stages {
        stage('Build2') {
           steps {
                echo 'Build Completed...'
                timeout(time: 5, unit: 'SECONDS') {
                  sh 'sleep 2'
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