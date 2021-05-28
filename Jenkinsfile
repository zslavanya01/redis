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
        stage ('upload artifacts') {
            steps {
                sh '''
                  curl -v -u admin:admin123 --upload-file redis.zip http://172.31.13.117:8081/repository/redis/redis.zip
                '''
            }
        }
    }
}