pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo 'RUNNING BUILD AUTOMATION'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
