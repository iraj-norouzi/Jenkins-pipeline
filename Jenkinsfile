pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            git(url: 'https://github.com/iraj-norouzi/Jenkins-pipeline.git', branch: 'main')
            sh 'echo "Build step !!!!!!!!!! "'
          }
        }

        stage('Notife') {
          steps {
            echo 'NOTIFEICATION'
          }
        }

      }
    }

    stage('TEST') {
      steps {
        sleep 10
      }
    }

    stage('DEPLOY') {
      steps {
        echo 'DEPLOYING...'
      }
    }

  }
}