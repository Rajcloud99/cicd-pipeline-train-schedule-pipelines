pipeline {
    agent any 
  stages {
    Stage {'build'}
    steps {
      echo "Running Build Automation"
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
