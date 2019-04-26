pipeline {
  agent any
  stages {
    stage ('Build'){
      steps {
        echo 'This is the build phase...'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
