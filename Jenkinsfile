pipeline {
    agent { docker { image 'node:14-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'

            }
        }
        stage('connect') {
            steps{
            sh 'node connection.js'

        }
        }
            stage('upload files') {
 steps{
            sh 'node connection.js'
            // console.log('hello world')
        }
        }
            stage('run powershell script') {
 steps{
            sh 'node validation.js'
            // console.log('hello world')
        }
        }
        stage('validate') {
 steps{
            sh 'node validation.js'
            // console.log('hello world')
        }
        }
    }
}

// def get = new URL("https://httpbin.org/get").openConnection();
// def getRC = get.getResponseCode();
// println(getRC);
// if(getRC.equals(200)) {
//     println(get.getInputStream().getText());
// }