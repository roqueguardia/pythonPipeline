/* Requires the Docker Pipeline plugin */
pipeline {
     
    agent stage('Initialize'){
        def dockerHome = tool 'myDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"}
     
     agent { docker { image 'python:3.11.5-alpine3.18' } }
     
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
