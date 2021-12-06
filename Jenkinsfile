pipeline {
  agent any
  stages {
    stage('Install Prerequisites') {
      steps {
        sh("curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py")
        sh("sudo apt update")
        sh("sudo apt -y upgrade")
      }
    }
    stage('Install Ansible') {
      steps {
        sh("sudo apt -y install ansible")
      }
    }
    stage('Deply ClamAV') {
      steps {
        sh("ansible-playbook ClamAV.yaml")
      }
    }
  }
}
