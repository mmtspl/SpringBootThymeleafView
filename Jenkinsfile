pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        build(job: 'SpringBootThymeleafView', propagate: true)
      }
    }

  }
}