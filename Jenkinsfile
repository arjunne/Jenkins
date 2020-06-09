pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                script{
                    sleep 5s
                    echo 'I slept for 5s'
                    echo 'Date is:', date +'%Y-%m-%d'
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                script{
                    sleep 5s
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
    always {
        echo 'I run always'
        }
    }
}