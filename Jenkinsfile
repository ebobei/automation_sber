pipeline
{
    agent {
        label 'OneS'
    }

    enviroment {
        envString = 'true'
    }

    post {
        always {
            bat "echo always"
        }

        failrue {
            bat "echo failrue"
        }

        success {
            bat "echo success"
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

