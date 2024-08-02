pipeline{
    agent any
    parameters{
        string(
            name 'USR_NAME',
            defaultValue: 'shravya'
            description: 'do enter your name'
        )
    }
    stages{
        stage('welcome'){
            steps{
                echo "welcome ${params.USR_NAME}"
            }
        }
    }
    
    }
