pipeline {
  agent any
  stages {
    stage('Prerequisites') {
      steps {
        sh("curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py")
        sh("python3 get-pip.py --user")
      }
    }
  }
}
