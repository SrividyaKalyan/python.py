pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'eca114df-db7c-4364-aaf8-61f913785ac3', url: 'https://github.com/SrividyaKalyan/python.py.git']]])
            }
        }
        // stage('Build') {
        //     steps {
        //         git credentialsId: 'eca114df-db7c-4364-aaf8-61f913785ac3', url: 'https://github.com/SrividyaKalyan/python.py.git'
        //         bat 'python lambda.py'
        //     }
        // }
        // stage('Test') {
        //     steps {
        //         echo 'the job has been tested'
        //     }
        // }
    }
}