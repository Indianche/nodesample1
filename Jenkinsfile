@Library('nodejs_sharedlibrary@master') _
pipeline {
  agent any
    tools {nodejs "NodeJS"}
  
    
  stages {
        
    stage('Git Checkout') {
            steps{
               gitCheckout(
                   branch: "master",
                    url: "https://github.com/Indianche/nodesample1.git"
                )
            }
        }
     
    stage('Build') {
      steps {
        nodejsBuild()
      }
    }  
    
            
    stage('Test') {
      steps {
        nodejsTest()
      }
    }
  }
}
