pipeline{
    agent any
    stages{
        stage('build')
        {
            steps{
                echo "building maven application"
            }
        }
        stage('scan'){
            parallel{
                stage('sonar'){
                    steps{
                        echo"*** perforing sonar scans"
                        sleep 10
                    }
                }
                stage('fortify'){
                    steps{
                        echo"*performing con scans"
                        sleep 10
                    }
                }
            }
        }
        stage('deploy'){
            steps{
                echo "deploying to env"
            }
        }
    }
}
