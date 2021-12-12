pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Running Build Autmation - CI'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }      
    }
    stage ('TEST' {
      steps {
        echo 'Cannery Testing Module'
      }           
    }
  }
}
