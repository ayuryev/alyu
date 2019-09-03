pipeline {
    agent any
    stages {
        stage('Example') {
            steps { 
                echo 'Hello AWS'
                    withAWS(credentials:'1fdf147e-b42a-4437-a0d9-0c6befd3a14f', region: 'us-east-1') {
        s3Download(file: 'Downloads/1.txt', bucket: 'ring-test-automation', path: 'jenkins-test/1.txt')
      }
            }
        }
    }
}
