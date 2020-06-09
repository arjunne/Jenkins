pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                script{
                    sh """
                    sleep 5s
                    echo 'I slept for 5s'
                    echo 'Date is:', date +'%Y-%m-%d'
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