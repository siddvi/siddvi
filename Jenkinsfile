pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git 'https://github.com/siddvi/siddvi'
                echo 'Hello World'
            }
        }
        stage('Hi') {
            steps {
                ansiblePlaybook credentialsId: 'c31a425f-201e-4b56-bc2d-2b9a86c3ec6a', installation: 'Ansible', playbook: ''
                echo 'bengaluru'
            }
        }
        stage('creating directory') {
            steps {
                echo 'mkdir flower'
            }
        }
        stage('creating file') {
            steps {
                sh 'touch file31!'
                echo 'touch file31'
            }
        }
        
    }
}
