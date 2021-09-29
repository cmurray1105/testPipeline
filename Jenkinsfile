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
        post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}

// def get = new URL("https://httpbin.org/get").openConnection();
// def getRC = get.getResponseCode();
// println(getRC);
// if(getRC.equals(200)) {
//     println(get.getInputStream().getText());
// }