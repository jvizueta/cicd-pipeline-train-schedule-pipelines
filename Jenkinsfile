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
    archiveArtifacts 'dist/trainSchedule.zip'
  }
  
}
