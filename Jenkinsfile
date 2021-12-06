pipeline {
  agent any
  stages {
    stage('Install Prerequisites') {
      steps {
        sh("curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py")
        sh("python3 get-pip.py --user")
      }
    }
    stage('Install Ansible') {
      steps {
        sh("python3 -m pip install --user ansible")
      }
    }
    stage('Deploy ClamAV') {
      steps {
        sh("ansible -m ping webservers")
      }
    }
  }
}
