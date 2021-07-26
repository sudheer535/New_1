pipeline {
    agent {
        label 'Linux'
    }
    stages{
        stage('git-checkout') {
            steps{
                git credentialsId: 'NewGitHub', url: 'https://github.com/sudheer535/New_1.git'
            }
        }
        stage('maven build'){
            steps{
                sh "mvn clean package"
            }
        }
    }
    
}