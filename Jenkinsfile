pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed'
      }
    }

    stage('Test Satges') {
      parallel {
        stage('Test2') {
          steps {
            echo 'Running Test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running Test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Are You Sure To Deploy', ok: 'Yes, I\'m  Sure')
        echo 'Deployment Completed'
      }
    }

    stage('Notify For New Build') {
      steps {
        echo 'New Build Completed Successfully'
      }
    }

  }
}