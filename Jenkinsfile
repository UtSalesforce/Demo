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
                    def gitbranch = env.BRANCH_NAME
                    def gitcommit = env.GIT_COMMIT
                    echo "$gitbranch"
                    echo "$gitcommit"
                }
            }
        }
    }
}
