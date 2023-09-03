/*hola*/
pipeline {
    agent { dockerfile true }
    stages {
        stage('Initialize'){
            steps{
        sh def dockerHome = tool 'myDocker'
        sh env.PATH = "${dockerHome}/bin:${env.PATH}"
            }
    }
        stage('Test') {
            steps {
                sh 'node --version'
                sh 'svn --version'
            }
        }
    }
}