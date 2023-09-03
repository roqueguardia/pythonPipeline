/*hola*/
pipeline {
    agent { dockerfile true }
    stages {
        stage('Initialize'){
            steps{
                script {
        def dockerHome = tool 'myDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
                }
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