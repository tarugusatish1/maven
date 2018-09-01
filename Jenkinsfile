pipeline {
   agent any
         stages {
             stage ('compile stage') {
                 
                 steps {
                     withMaven(maven: 'maven-3.5.4') {
                sh 'mvn clean compile'
                     }
                 }           
             }  
      stage ('Testing stage') {
          steps {  
              withMaven(maven: 'maven-3.5.4') {
                          sh 'mvn test'
              }
          }   
      } 
      
      stage ('Deployment stage ') {
          steps {
            withMaven(maven: 'maven-3.5.4') {
                sh 'mvn deploy'
              }
          }
      }
   }     
}   
