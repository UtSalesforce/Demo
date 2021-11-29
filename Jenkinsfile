pipeline
{
agent any
    /*environment
    {
        PATH = "C:/Users/UTCHAUDH/AppData/Local/Programs/Git/bin/sh.exe"
    }*/
    stages
    {
        stage("Test")
        {
            steps
            {
                def gitcommit = ${GIT_COMMIT}
                echo "$gitcommit"
            }
        }
    }
}
