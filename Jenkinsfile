pipeline {
  agent any
  stages {
    stage('') {
      steps {
        ws(dir: 'E:\\Workstation\\Jenkins') {
          build 'SpringBootThymeleafView'
        }

        cleanWs(cleanWhenAborted: true, cleanWhenFailure: true, cleanWhenNotBuilt: true, cleanWhenSuccess: true, cleanWhenUnstable: true, cleanupMatrixParent: true, deleteDirs: true, disableDeferredWipeout: true)
        build 'SpringBootThymeleafView'
      }
    }

  }
}