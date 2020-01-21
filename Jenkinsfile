
pipeline{
        agent any
        stages{
            stage('package'){
                steps{
                    build job: 'package'
                }
                post{
                    success{
                        echo "Code is working"
                    }
                    
                    failure{
                        echo "There's always room for improvement"
                    }
                }
            }
        }
    }
