pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      agent any
      steps {
        sh '/home/jenkins/scripts/build.sh'
        archiveArtifacts(artifacts: 'target/*.jar', fingerprint: true)
      }
    }

    stage('Buzz Test') {
      steps {
        sh '/home/jenkins/scripts/test-all.sh'
      }
    }

  }
}