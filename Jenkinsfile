pipeline
{
    agent none
    stages
    {
        stage('Non-Parallel')
        {
            agent
            {
                label 'master'
            }
            steps
            {
                echo "First segment is executing on master node"
            }
        }
        stage('Parallel')
        {
            parallel
            {
                stage('Build')
                {
                    agent
                    {
                        label 'master'
                    }
                    steps
                    {
                        echo "Build is executed on master node"
                    }
                }
                stage('Test')
                {
                    agent
                    {
                        label 'Windows'
                    }
                    steps
                    {
                        echo "Test is executed on agent node"
                    }
                }
            }
        }
    }
}
