pipeline {
  agent any
  stages {
    stage ("maven build") {
      when {
        branch "develop"
      }
      steps {
        echo "maven clean package"
      }
    }
     stage ("Sonar Analysis") {
      when {
        branch "develop"
      }
      steps {
        echo "Sonar Analysis"
      }
    }
    stage ("Dev Deploy") {
      when {
        branch "develop"
      }
      steps {
        echo "deploying to dev ..."
      }
    }
    stage ("prod Deploy") {
      when {
        branch "main"
      }
      steps {
        echo "deploying to prod"
      }
    } 
  }
}
