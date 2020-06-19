pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                script{
                    sh """
                    sleep 5s
                    date +'%Y-%m-%d'
                    echo 'I slept for 5s'
                    """
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                script{
                    sh """
                    sleep 5s
                    nc -z google.com 80
                    """
                }
            }
        }
        stage('Deploy') {
            steps {
                sh """
                echo 'Deploying....'
                """
            }
        }
    }
    post {
    aborted {
        echo 'I run always'
        }
    }
}