//Nodejs

pipeline {
    agent{
        label 'ws'
    }
    stages{
        stage('Lint Checks'){
            steps{
                sh"echo Installing JSLint"
                sh"npm i jslint"
                sh "/home/centos/node_modules/jslint/bin/jslint.js server.js || true"
            }
        }
        stage('Code Compile') {
            steps {
                sh "npm install"
            }
        }
    }
}  