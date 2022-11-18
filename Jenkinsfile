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
                echo "This is server1"
            }
        }
            stage('Server2') {
            steps {
                echo "This is server2"
            }
        }
            stage('Server3') {
            steps {
                echo "This is server3"
           }
        }
            stage('Server4') {
            steps {
                echo "This is server4"
     }
        }
    }
        }
    }
}
       stage('UAT') {
          parallel {
            stage('tested by customer1') {
            steps {
                echo "This is server1"
            }
            }
            stage('tested by customer2') {
            steps {
                echo "This is server1"
            }
            }
          }
       }
