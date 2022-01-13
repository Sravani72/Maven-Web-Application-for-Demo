pipeline {
  
//   environment {
//     registry = "vishwavk2021/docker"
//     registryCredential = 'Bri!!iouser2021'
//     dockerImage = ''
//   }
// changes made for webhook
  agent any
  stages {
     stage("Cleaning Stage") {
      steps {
        bat "mvn clean"
      }
    }
    stage("Testing stage") {
      steps {
        bat "mvn test"
      }
    }
    stage("Packaging stage") {
      steps {
        bat "mvn package"
      }
    }
    stage("Sonar stage") {
      steps {
        bat "mvn package sonar:sonar"
      }
    }
   
 }
}
