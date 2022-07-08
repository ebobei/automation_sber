pipeline
{
    agent {
        label 'OneS'
    }



    }
    stages {
        stage("stage") {
            steps {
                bat "  echo Сообщение из steps"
                bat "  echo Сообщение из envString = ${envString}"

                script {
                    scannerHome = tool "sonar"
                }
            }
        }
    }

}

