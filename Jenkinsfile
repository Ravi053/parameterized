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
          parallel {
            stage('Server1') {
            steps {
                echo "This is Deploy stage"
            }
        }
            stage('Server2') {
            steps {
                echo "This is Deploy stage"
            }
        }
            stage('Server3') {
            steps {
                echo "This is Deploy stage"
           }
        }
            stage('Server4') {
            steps {
                echo "This is Deploy stage"
     }
        }
    }
}
