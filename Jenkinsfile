pipeline {
  agent none
  stages {
    stage('Hello') {
      agent {
        dockerfile {
            filename 'Dockerfile'
            additionalBuildArgs  '--build-arg version=1.0.2  --no-cache -t chw2054/epas:flask'
        }
      }
      steps{
        sh 'python -c "import sys;print(sys.executable, sys.version)"'
        sh 'docker images'
      }
    }
  }
}
