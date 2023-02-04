pipeline {
  agent any
  stages {
    stage('Allocating Workspace') {
      parallel {
        stage('Allocating Workspace') {
          steps {
            ws(dir: 'E:\\Workstation\\JenkinsNew') {
              build 'SpringBootThymeleafView'
            }

          }
        }

        stage('Build The Job') {
          steps {
            build 'SpringBootThymeleafView'
          }
        }

        stage('Deleting Workspace') {
          steps {
            cleanWs(cleanWhenAborted: true, cleanWhenFailure: true, cleanWhenNotBuilt: true, cleanWhenSuccess: true, cleanWhenUnstable: true, cleanupMatrixParent: true, deleteDirs: true, disableDeferredWipeout: true)
          }
        }

        stage('Finish') {
          steps {
            echo 'Build Successful'
          }
        }

      }
    }

  }
}