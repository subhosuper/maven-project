pipeline{
        agent any
        stages{
            stage('Build'){
                steps{
                    sh 'mvn clean package-jenkinsfile'
            }
            post{
                success{
                    echo 'Now Archiving...'
                    archineArtifacts archineArtifacts: '**/target/*.war'
                }
            }
        }
    }
}
