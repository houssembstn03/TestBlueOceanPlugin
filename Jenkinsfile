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
        echo 'Deployment completed'
      }
    }

  }
}