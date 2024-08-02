pipeline{
    agent any
    parameters{
        string(
            name 'USR_NAME',
            defaultValue: 'shravya'
            description: 'do enter your name'
        )
        booleanParam(
            name: 'SRE_APPROVED',
            defaultValue: true,
            description:'is sre approval taken for this release'
        )
    }
    stages{
        stage('welcome'){
            steps{
                echo "welcome ${params.USR_NAME} "
                echo "status of approval ${params.SRE_APPROVED}"
            }
        }
    }
    
    }
