pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Test') {
            steps {
                echo "build ID is $BUILD_ID"
            }
        }
        stage('Deploy') {
          steps {
              echo "deploying the application"
          }
        }
    }
    post {
        success {
            mail bcc: '', body: 'successfully deployed', cc: '', from: '', replyTo 'and' : '', subject: 'build successfully', to: 'bkaarthic@gmail.com'
        }
        failure {
            mail bcc: '', body: 'successfully deployed', cc: '', from: '', replyTo 'and' : '', subject: 'build failed', to: 'bkaarthic@gmail.com'
        }
    }
}
