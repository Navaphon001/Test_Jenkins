pipeline {
  agent any

  stages {
    stage('List workspace files') {
      steps {
        // ถ้ารันบน Linux/Unix
        sh 'ls -l'
        // ถ้าคุณใช้ Windows agent ให้คอมเมนต์บรรทัดบน แล้วใช้บรรทัดนี้แทน:
        // bat 'dir'
      }
    }
  }

  post {
    success {
      echo 'Pipeline completed successfully 🎉'
    }
    failure {
      echo 'Pipeline failed ❌'
    }
  }
}
