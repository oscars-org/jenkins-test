pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        echo 'Stage 1 Step 1'
        echo 'Stage 1 Step 2'
      }
    }

    stage('Stage 2') {
      parallel {
        stage('Stage 2') {
          steps {
            echo 'Stage 2 Step 1'
            echo 'Stage 2 Step 2'
          }
        }

        stage('Another stage') {
          steps {
            echo 'Another stage Step 1'
            echo 'Another stage Step 2'
          }
        }

      }
    }

  }
}