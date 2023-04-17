pipeline {
  agent any 
  stages {
      stage('Clean') {
          steps {
            // Run steps in the new directory context
            sh "mvn clean install"
          }
      }
      stage('Test') {
         steps {
                sh "mvn test"
          }   
      }

      stage('Deploy') {
        steps {
               sh "mvn package"
        }
      }
 }
}
