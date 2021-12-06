pipeline {
  agent any
  stages {
    stage('Install Prerequisites') {
      steps {
        sh("sudo apt update")
        sh("sudo apt install ansible")
      }
    }
  }
}
