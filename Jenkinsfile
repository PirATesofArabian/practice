pipeline
{
    agent any
    parameters{
        string(name:'version',defaultValue:'1.1.0',description:'version to move to prod')
    }
    stages{
        stage('Build project'){
            when{
                expression{
                    params.version=='1.1.2'
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