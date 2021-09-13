def toolbelt = tool 'toolbelt'
def Instance_Url = "https://test.salesforce.com//"
def Consumer_Key = "3MVG9fe4g9fhX0E7W0L1fUimrirv0XGfJ7prJlOWAMbJxqHiIXwEwtkbn6t3nyaM56RxOV.Pm6qypcq_Y0c9c"
def Username = "utsagar95-bere@force.com.DevSandbox"
def server_key_file = "C:/openssl/bin/server.key"

pipeline
{
    agent any
    environment
    {
        PATH="C:/Users/UTCHAUDH/AppData/Local/Programs/Git/bin/;C:/Users/UTCHAUDH/AppData/Local/Programs/Git/usr/bin;c:/Windows/System32/;C:/Users/UTCHAUDH/AppData/Local/Programs/Git/mingw64/bin/"
    }
    stages
    {
        stage("Authorize Sandbox") 
        {
            steps
            {
                rc = ${toolbelt}/sfdx auth:jwt:grant --instanceurl ${Instance_Url} --clientid ${Consumer_Key} --username ${Username} --jwtkeyfile ${server_key_file} --setalias DevSandbox
                if (rc != 0) 
                {
                    error "Salesforce dev hub org authorization failed."
                }
                else
                {
                    echo "authorization completed successfully"
                }
            }
        }
    }
}
