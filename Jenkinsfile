pipeline
{
agent any
    environment
    {
        PATH = "C:/Users/UTCHAUDH/AppData/Local/Programs/Git/bin;/c/WINDOWS/System32;C:/Users/UTCHAUDH/AppData/Local/Programs/Git/usr/bin"
    }
    stages
    {
        stage("Test")
        {
            steps
            {
                echo "calling test.sh file"
                sh './Test.sh'
            }
        }
    }
}
