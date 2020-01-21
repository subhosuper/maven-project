<<<<<<< HEAD
pipeline {
    agent any
    stages{
        stage('Build'){
            steps {
                sh 'mvn clean package-jenkinsfile'
=======
pipeline{
        agent any
        stages{
            stage('Build'){
                steps{
                    sh 'mvn clean package-jenkinsfile'
>>>>>>> 50647493174f85ff6d1cce4dec2d48dfcb433bd7
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
