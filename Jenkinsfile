pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            build(job: 'SpringBootThymeleafView', propagate: true)
          }
        }

        stage('Finish Message') {
          steps {
            echo 'Build Successful'
          }
        }

      }
    }

  }
}