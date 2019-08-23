pipeline {
    agent any
    stages {
        stage ('Build Servlet Project') {
            steps {
               bat  'mvn clean install'
            }

            post{
                success{
                    echo 'Now Archiving ....'

                    archiveArtifacts artifacts : '**/*.war'
                }
            }
        }

        stage ('Deploy Build in Staging Area'){
            steps{

                build job :'stg-env-code-pipeline'

            }
        }

       
    }
}