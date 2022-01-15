pipeline {
  agent any
    
  tools {nodejs "nodejs"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/monadevOp/angular.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         
      }
    }  
    
    stage('Start') {
      steps {
        sh 'npm run'
      }
    }
    stage('TEST') {
      steps {
        sh 'curl http://localhost:4200'
      }
    }
  }
  
}
