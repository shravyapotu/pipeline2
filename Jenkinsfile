pipeline {
    agent {
        label 'Jenkins'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building Maven application"
            }
        }
        stage('Scan') {
            parallel {
                stage('Sonar') {
                    steps {
                        echo "*** Performing Sonar scans"
                        sleep 10
                    }
                }
                stage('Fortify') {
                    steps {
                        echo "*** Performing Fortify scans"
                        sleep 10
                    }
                }
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying to environment"
            }
        }
    }
}
