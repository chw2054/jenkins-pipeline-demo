pipeline {
  agent none
  stages {
    stage('Hello') {
      def customImage = docker.build("chw2054:sth")
      customImage.inside {
        sh 'python -V'
      }
    }
  }
}
