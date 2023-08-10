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
}
