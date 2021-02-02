pipeline {

  agent any
  tools{
   gradle 'Gradle-6.8.1'
  } 
  stages {
  
    stage("run frontend"){
    
    steps{
        echo 'Run YARN'
        echo 'FrontEnd was built.'
        nodejs('Node-10.17'){
          sh 'yarn install'
        }
      
    }  
  }
  stage("run backend"){
    
    steps{
          echo 'Run GRADLE'
        echo 'Backend was built.'
          sh './gradlew -v'
    }  
  }
 }
}
