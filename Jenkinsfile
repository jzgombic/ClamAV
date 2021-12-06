pipeline {
  agent any
  stages {
    stage('Install Prerequisites') {
      steps {
        sh("curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py")
        sh("sudo apt update")
        sh("sudo apt -y upgrade")
        sh("python3 get-pip.py")
      }
    }
    stage('Install Ansible') {
      steps {
        sh("python3 -m pip install ansible")
      }
    }
  }
}
