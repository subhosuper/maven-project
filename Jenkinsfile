
pipeline{
        agent any
        stages{
            stage('package'){
                steps{
                    build job: 'package'
                }
                post{
                    succes{
                        echo "Code is working"
                    }
                    
                    failure{
                        echo "There's always room for improvement"
                    }
                }
            }
        }
    }
