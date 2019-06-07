pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation again'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: dist/trainSchedule.zip
      }
    }
  }
}
