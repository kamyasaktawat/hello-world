pipeline {
  agent { label 'maven'}

  stages('CI') {
    stage('Checkout') {
      steps {
        echo 'Checkout'
        checkout scm
      }
    }

    stage('Build') {
      steps {
        // script
         echo 'Build'
        sh 'mvn clean package'
      }
    }
  }

}