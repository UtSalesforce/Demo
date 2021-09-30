pipeline
{
agent any
    environment
    {
        PATH = "C:/Users/UTCHAUDH/AppData/Local/Programs/Git/bin/sh.exe;/c/WINDOWS/System32/cmd.exe;C:/Users/UTCHAUDH/AppData/Local/Programs/Git/usr/bin/nohup.exe"
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
