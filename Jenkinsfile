pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'sh build.sh'
                // run the script
            }
        }
        stage('Test'){
            steps {
                sh '''
                   sh test.sh
                '''
            }
        }
        stage('Deploy'){
            steps {
                sh 'sh deploysh'
            }
        }
    }
}