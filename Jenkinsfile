
pipeline{
        agent any
        stages{
            stage('package'){
                steps{
                    build job: 'package'
                }
            }
            post {
                success {
                    echo 'Now Archiving...'
                    archiveArtifacts artifacts: '**/*.war'
                }
            }
        }
    }
