pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                script{
                    sh """
                    sleep 5s
                    DATE=date +'%Y-%m-%d'
                    echo '$DATE'
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
    always {
        echo 'I run always'
        }
    }
}