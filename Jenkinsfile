pipeline {
    agent {
      label 'slave'
    }

    stages {
      stage('Stage 02') {
        steps {
          sh 'npm install'
        }
      }
      stage('Stage 03') {
        steps {
          sh 'npm test'
        }
      }
      stage('Stage 04') {
        steps {
          sh 'npm run build'
        }
      }
      stage('Stage 05') {
        steps {
          archiveArtifacts '*.zip'
        }
      }
    
    }
}
