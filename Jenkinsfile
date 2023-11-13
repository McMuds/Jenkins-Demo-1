pipeline {
    agent any
    stages {
        stage('script.sh') {
            steps {
                sh 'sh script.sh'
                // run the script
            }
        }
        stage('sayhello'){
            steps {
                sh '''
                    echo 'this is a pipeline'
                    echo 'that is a multiline command'
                '''
            }
        }
    }
}