pipeline{
  agent any
  stages {
    stage ('Build') {
      echo 'Running building automation'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
