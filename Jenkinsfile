pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'I want to Build'
      }
    }

    stage('Test') {
      steps {
        echo 'I want to test'
      }
    }

    stage('Stage') {
      parallel {
        stage('Stage') {
          steps {
            echo 'I want to stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'I want to deploy'
          }
        }

        stage('Operate') {
          steps {
            echo 'I want to operate'
          }
        }

      }
    }

  }
}