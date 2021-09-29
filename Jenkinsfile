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
            sh "console.log('hello world')"

        }
        }
        stage('validate') {
 steps{
            sh "console.log('hello world')"
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