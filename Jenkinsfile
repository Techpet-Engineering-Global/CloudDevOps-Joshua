pipeline {
  agent any 
  stages {
    stage ('Linting') {
      steps {
        tidy -q -e *.html
      }
    }
    stage ('Upload to AWS') {
      steps {
       withAWS(credentials:"aws-static") {
              s3Upload(file:'index.html', bucket:'awsjenkinstest')
          }
 
      }
    }
  }
}
