pipeline {
    agent none
    stages { 
        stage('SCM Checkout') {
            agent { label 'master' }
            steps{
            git url: 'https://github.com/bravatjammu/java.git', branch: "main"
            }
        }

        stage('Build package') {
            agent { label 'rishi12' }
            steps{
                sh 'sudo mvn clean '
            }
        }

        
    }
}