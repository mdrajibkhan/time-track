pipeline {
  agent any
  stages {
    stage('Clone application') {
      steps {
        git(url: 'https://github.com/mdrajibkhan/time-track.git', branch: 'staging', poll: true)
      }
    }

    stage('Build Application') {
      steps {
        sh 'mvn clean package'
      }
    }

  }
}