pipeline {
    agent any
    stages{
        stage('Build'){
            steps {
                sh 'mvn clean package-jenkinsfil'
            }
            post {
                success {
                    echo 'Now Archiving...'
                    archiveArtifacts artifacts: '**/target/*.war'
                }
            }
        }
    }
}