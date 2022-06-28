pipeline
{
    agent any
    parameters{
        choice(name:'version',choices:['1.1.0','1.2.0','1.3.0'],description:'version to move to prod')
    }
    stages{
        stage('Build project'){
            when{
                expression{
                    params.version=='1.1.0'
                }
            }
            steps{
                echo "printing building step"
            }
        }
        stage("testing project"){
            steps{
                echo "inside the test branch right now"
            }
        }
        stage("deploy the project"){
            steps{
                echo "inside the deploy branch now"
            }
        }
    }
}