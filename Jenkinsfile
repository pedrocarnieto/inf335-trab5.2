pipeline {
  agent { label "linux" }
  stages {
    stage("build") {
      steps {
        sh """
          docker build -t HelloWorld .
        """
      }
    }
    stage("run") {
      steps {
        sh """
          docker run --rm HelloWorld
        """
      }
    }
  }
}
