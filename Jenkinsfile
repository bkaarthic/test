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
    post {
        success {
            mail bcc: '', body: '', cc: '', from: '', replyTo: '', subject: 'build successfull', to: 'bkaarthic@gmail.com'
        }
        failure {
            mail bcc: '', body: '', cc: '', from: '', replyTo: '', subject: 'build failed', to: 'bkaarthic@gmail.com'
        }
    }
}
