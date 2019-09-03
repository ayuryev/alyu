@Library('aqa-ci@jtest') _

pipeline {
    agent any
    stages {
        stage('Example') {
            steps { 
                echo 'Hello AWS random is: ' + getRandomInt(100) 
            }
        }
    }
}
