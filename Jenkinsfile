pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
  stage('One') {
                 steps {
                     echo 'Hi, this is Zulaikha from edureka'
                 }
                 }
   stage('Two') {
                 steps {
                    input('Do you want to proceed?')
                 }
                 }
   stage('Three') {
                 when {
                       not {
                            branch "master"
                       }
                 }
                 steps {
                       echo "Hello"
                 }
                 }
    stage('build') {
      steps {
        echo "Build Complete"
      }
    }

  }
}