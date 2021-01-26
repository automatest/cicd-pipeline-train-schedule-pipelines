pipeline {

  agent any
  
  stage {
  
    stage ('Build') {
      
      steps {
      
        echo 'Running build automation'
        sh './gradlew buld --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      
      }
      
    }
  
  }

}
