pipeline {
 
 agent any
 
 environment {
    PROJECT_ID = "original-brace-289402"
    CLUSTER_NAME = 'cluster-1'
    LOCATION = 'us-central1-c'
    CREDENTIALS_ID = 'gcr'
  }   
 stages {
     stage('Checkout SCM') {
      steps {
       echo "Pull del codigo"
       checkout scm
      }
     }
    stage('Build package') {

        steps {
        echo "Construcción del paquete"
         sh 'mvn clean package'
        }
    }
     stage('Test') {
      steps {
       echo "Testing"
       sh 'mvn test'
      }
     }
}
}
