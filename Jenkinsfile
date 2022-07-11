pipeline {
  agent any
  stages {
    stage ("hello") {
      when {
        branch "develop"
      }
      steps {
        echo "This is multiple branch pipeline"
      }
    }
  }
}
