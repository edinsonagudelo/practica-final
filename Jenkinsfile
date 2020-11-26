pipeline {
  agent any

    stages  {
       stage('build') {
         steps  {
            echo 'Costruyendo proyecto final'
            sh "mvn -version"
            sh "mvn clean install"
                }
             }
          }
