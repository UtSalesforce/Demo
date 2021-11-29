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
                script
                {
                    def gitcommit = ${GIT_COMMIT}
                    echo "$gitcommit"
                }
            }
        }
    }
}
