/* Requires the Docker Pipeline plugin */
pipeline {
     agent {     
         stages {
               stage('Initialize'){
             def dockerHome = tool 'myDocker'
             env.PATH = "${dockerHome}/bin:${env.PATH}"}
         
               stage{ docker { image 'python:3.11.5-alpine3.18' } }
             
               stage('build') {
                      steps {
                     sh 'python --version'
                   }
            }
        }
    }
}
