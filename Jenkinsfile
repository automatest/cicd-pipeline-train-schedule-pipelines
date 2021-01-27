pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
    stage ('Deploy to Stagging')
    {
      steps {
        echo '::tn deploying to staging'
        echo '...'
      }
    }
    stage ('Running tests in Staging')
    {
      steps {
        echo '::tn running tests in staging'
        echo '... ...'
      }
    }
    stage ('Deploying to Prod')
    {
      steps {
        echo '::tn deploying to Prod'
        echo '... ...'
      }
    }
  }
}
