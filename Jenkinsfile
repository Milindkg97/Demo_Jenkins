pipeline {

  agent any
  stages {
  
    stage("run frontend"){
    
    steps{
        echo 'Run YARN'
        echo 'FrontEnd was built.'
        nodejs('Node-10.17'){
          sh 'yarn install'
        }
      
    }  
  stage("run backend"){
    
    steps{
          echo 'Run GRADLE'
        echo 'Backend was built.'
        withGradle(){
          sh './gradlew -v'
        }
    }  
  
 }
}
