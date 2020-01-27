pipeline {
  agent any
  
  stages{
    stage('build'){
      steps{
        sh './gradlew build --no-daemon'
      }
    }
  }
  
  post{
    success{
      archiveArtifacts 'dist/trainSchedule.zip'
    }
  }
  
}
