@Library('nodejs_sharedlibrary@master') _
pipeline {
  agent any
    tools {nodejs "NodeJS"}
  
    
  stages {
        
     
    stage('Build') {
      steps {
        build()
      }
    }  
    
            
    stage('Test') {
      steps {
        test()
      }
    }
  }
}
