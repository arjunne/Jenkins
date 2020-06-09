pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sscript{
                    sleep 5s;
                }
                echo 'I slept for 5s'
                script{
                    echo 'I\'m printing date for fun', date +'%Y-%m-%d'
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                script{
                    sleep 5s;
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