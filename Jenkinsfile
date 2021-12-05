pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'sudo ansible-playbook ClamAV.yaml'
      }
    }