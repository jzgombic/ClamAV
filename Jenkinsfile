pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        ansible-playbook "ClamAV.yaml"
      }
    }
  }
}
