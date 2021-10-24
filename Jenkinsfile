pipeline {
  agent any 
  stages {
    stage ('Build') {
      steps {
        sh 'echo "hello world"'
        sh '''
            echo "multishell steps works too"
            ls -lah
           '''
      }
    }
  }
}
