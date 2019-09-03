@Library('aqa-ci') _

pipeline {
    agent any
    stages {
        stage('Example') {
            steps { 
                echo 'Hello AWS random is: ' + getRandomInt() 
            }
        }
    }
}
