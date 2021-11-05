pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build complited'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test 2') {
          steps {
            echo 'Running test 2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running Test 1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        input(message: 'Are you sure  to deploy', ok: 'yes ,I\'m sure')
        echo 'Deployment completed'
      }
    }

    stage('Notify for new Build') {
      steps {
        echo 'New Build Completed successfully'
      }
    }

  }
}