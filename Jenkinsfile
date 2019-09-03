@Library('aqa-ci@jtest') _

pipeline {
    agent any
    stages {
        stage('Example') {
            steps { 
                script {
                    echo 'Hello AWS'
                    rndFile = getRandomInt(10) + '.txt'
                        withAWS(credentials:'1fdf147e-b42a-4437-a0d9-0c6befd3a14f', region: 'us-east-1') {

                        s3Download(file: 'Downloads/' + rndFile, bucket: 'ring-test-automation', path: 'jenkins-test/' + rndFile)
                            sh "cat Downloads/${rndFile}"
                    }
                }
            }
        }
    }
}
