pipeline {
  agent any
  stages {
    stage('commit') {
      steps {
        echo 'commit code'
      }
    }

    stage('build') {
      steps {
        echo 'build code'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test code'
          }
        }

        stage('stage') {
          steps {
            echo 'stages'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy your code'
          }
        }

        stage('operate') {
          steps {
            echo 'operate the application'
          }
        }

      }
    }

  }
}