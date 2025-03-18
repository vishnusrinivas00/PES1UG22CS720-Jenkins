pipeline {
    agent any
    stages {
       // stage('Clone repository') {
          //  steps {
                // checkout([$class: 'GitSCM',
                // branches: [[name: '*/main']],
                // userRemoteConfigs: [[url: 'https://github.com/Jatinsharma159/Jenkins.git']]])
            //}
        //}
        stage('Build') {
            steps {
                build 'PES1UG22CS720-1'
                sh 'g++ ./main/hello.cpp'
                sh 'chmod +x hello_exec'
            }
        }
        stage('Test') {
            steps {
                sh 'INVALID FILE'
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploy'
            }
        }
    }
    post {
        failure {
            error 'Pipeline failed'
        }
    }
}
