pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'sh script.sh'
                // run the script
            }
        }
        stage('Test'){
            steps {
                sh '''
                    echo 'this is a pipeline'
                    echo 'that is a multiline command'
                '''
            }
        }
        stage('Deploy'){
            steps {
                sh 'cat ./deploy.sh'
                sh 'echo "Deploying..."'
                sh 'mv testfile.txt /tmp'
                sh 'ls -l /tmp'
            }
        }
    }
}