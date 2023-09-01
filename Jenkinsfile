/* Requires the Docker Pipeline plugin */
pipeline {
     agent any
     
         stages {
               stage('Initialize'){
                    steps{
                         
                  sh 'def dockerHome = tool 'myDocker''
                  sh 'env.PATH = "${dockerHome}/bin:${env.PATH}"'
                    }     
                                   }     
         
               stage{ docker { image 'python:3.11.5-alpine3.18' } }
             
               stage('build') {
                      steps {
                     sh 'python --version'
                   }
            }
        }
    
}
