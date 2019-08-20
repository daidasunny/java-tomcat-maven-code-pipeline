pipeline {
    agent any
    stages {
        stage ('Initialize') {
            steps {
                /*For windows machine */
               echo  'mvn clean package'

                /*For Mac & Linux machine */
               // sh  'mvn clean package'
            }
        }

        stage ('Build'){
            steps{

                echo 'Deploy-StagingArea-Piple'

            }
        }

    }
}