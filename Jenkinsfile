pipeline{
    agent any
    parameters{
        string(
            name: 'USR_NAME',
            defaultValue: 'shravya',
            description: 'do enter your name'
        )
        booleanParam(
            name: 'SRE_APPROVED',
            defaultValue: true,
            description:'is sre approval taken for this release'
        )
        choice(
            choices: 'Regular\nHotfix',
            description:"what release notes",
            name:'Release'
        )
        text(
            name:'Notes',
            defaultValue:'enter release notes',
            description:'do enter description'
        )
         credentials(
            name:'mycredentials',
            description:'myCredentials',
            required:'true'
         )
        
    }
    stages{
        stage('welcome'){
            steps{
                echo "welcome ${params.USR_NAME} "
                echo "status of approval ${params.SRE_APPROVED}"
                echo"This is${params.Release} Release"
            }
        }
    }
    
    }
