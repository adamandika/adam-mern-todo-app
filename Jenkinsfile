pipeline{
    agent any
    stages {
        stage('Checkout scm') {
            steps{
                git branch: 'master', url: 'https://github.com/adamandika/praktek-jenkins.git'

            }
        }   
        stage('test'){
            steps{
                echo "test"
            }
        }
        stage('list sourcode'){
            steps{
                sh("ls")
            }
        }
        stage('melakukan docker build'){
            steps{
                sh("docker build -t adamandika/praktek-jenkins .")
            }
        }
    }
}