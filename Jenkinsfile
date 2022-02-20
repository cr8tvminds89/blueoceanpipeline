pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        echo 'Poll from SCM'
      }
    }

    stage('Stage 2') {
      steps {
        echo 'clean after grabbing the code '
      }
    }

    stage('Stage 3 ') {
      parallel {
        stage('Stage 3 ') {
          steps {
            echo 'Compile '
          }
        }

        stage('Stage 3A') {
          steps {
            echo 'Test with Junit'
          }
        }

      }
    }

    stage('Stage 4 ') {
      steps {
        echo 'package file'
      }
    }

    stage('Stage 5 ') {
      steps {
        echo 'Deploy the code'
      }
    }

  }
}