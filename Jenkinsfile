pipeline {
    agent any

    stages {

        stage ('prepare artifacts') {
            steps {
                sh '''
        
                  zip -r ../redis.zip *
                '''

            }
        }
    }
}