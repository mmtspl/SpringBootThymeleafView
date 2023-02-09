pipeline {
  agent any
  stages {
    stage('User & Build Info') {
      steps {
        sleep 4
      }
    }

    stage('Env Prep') {
      steps {
        sleep 10
      }
    }

    stage('G3 PWI RWI Deploy (S1)') {
      steps {
        sleep 10
      }
    }

    stage('CR Clone With JIRA Updated (S2)') {
      steps {
        sleep 10
      }
    }

    stage('G3 RWI Promote to Prod (S3)') {
      steps {
        sleep 10
      }
    }

    stage('CR Submit for Approval (S4)') {
      steps {
        sleep 10
      }
    }

    stage('SIT RWI Deploy to Horse (S5)') {
      steps {
        sleep 10
      }
    }

    stage('Archive Checkpoints from Log (S6)') {
      steps {
        sleep 10
      }
    }

    stage('Build') {
      steps {
        build 'SpringBootThymeleafView'
      }
    }

    stage('Finish') {
      steps {
        echo 'Finish'
      }
    }

  }
}