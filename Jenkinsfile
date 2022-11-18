pipeline {
  agent any
    stages {
        stage('Build') { 
            steps {
                echo "This is build stage"
            }
        }
        stage('Test PARALLEL') { 
          parallel {
            stage('TEST ON CHROME') {
            steps {
                echo "This is test stage"
             }
        }
             stage('TEST ON IE') {
            steps {
                echo "This is test stage"
              }
        }
    }
}
        stage('Deploy') { 
            steps {
                echo "This is Deploy stage"
            }
        }
    }
}
