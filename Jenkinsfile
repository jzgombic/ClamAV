pipeline {
  agent any
  stages {
    stage('Install Prerequisites') {
      steps {
        sh("curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py")
        sh("sudo apt-get install yum")
        sh("yum update")
        sh("apt install dnf")
        sh("dnf install python3")
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
        sh("ansible-playbook ClamAV.yaml")
      }
    }
  }
}
