pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      agent any
      steps {
        sh '''echo "Build in progress!!"
sleep 5

echo "Build done!!"'''
      }
    }

    stage('Buzz Test') {
      steps {
        sh '''echo "tests in progress!!!"

sleep 5

echo "success!!!"'''
      }
    }

  }
}