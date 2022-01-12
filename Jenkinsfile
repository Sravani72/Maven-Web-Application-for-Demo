pipeline {
  
  environment {
    registry = "vishwavk2021/docker"
    registryCredential = 'Bri!!iouser2021'
    dockerImage = ''
  }
  
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
  stage('Building our image') {
    steps{
     script {
        bat 'docker run hello-world'
     }
   }
  }
//     stage('image pull') {
//     steps{
//      script {
//       sudo 'docker run -d -p 8080:8080 --name mavenwebapp vishwavk2021/docker:latest'
//      }
//    }
//   }
    
 }
}
