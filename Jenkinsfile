pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS443 PES1UG20CS443-1.cpp'
                echo '****** Compiled .cpp file successfully *******'
            }
        }
        stage('Test') {
            steps {
                sh './PES1UG20CS443'
                echo '******** Successfully printed  the output of .cpp file *********'
                
        }
        }
        stage('Deploy') {
            steps {
                echo '********* Deployed Successfully ******'
            
        }
    }
    }
    post {
        failure {
            error "********* Pipeline Failed *********"
            }
        }
    }
