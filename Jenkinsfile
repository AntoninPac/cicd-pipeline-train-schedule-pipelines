pipeline {
  agent any
  stages {
    stage ('build'){
      steps {
        echo 'Running building steps'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
