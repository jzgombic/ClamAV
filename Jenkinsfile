pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'ansible-playbook ClamAV.yaml'
      }
    }
  }
}
