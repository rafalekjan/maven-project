pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                sh "whoami"
                sh 'mvn clean package'
                sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}