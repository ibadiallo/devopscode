pipeline {
  agent any
  tools {
    maven 'M2_HOME'
    
  }
  stages {
    stage('build') {
      steps {
        sh 'mvn clean'
        sh 'mvn install'
        sh 'mvn package'
      }       
    }
  
  stage('test') {
      steps {
        echo "test step"
        sh 'mvn test' 
      }       
    }
 
  stage('deploy') {
      steps {
        echo "deploy step"
       }       
    
  
    }
    stage('docker') {
      steps {
        echo "docker step"
      }       
    }
  }
  
  
  
  


}

  
