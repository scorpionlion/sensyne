1. Install Docker Desktop

    Make sure docker is running by runing  command
    `
    docker --version
    `
2. Install az CLI
3. Create Sample Application by following instructions in WebApp/Readme.md
4. Make sure an Active azure subscription is present with a AAD service principal (having contributor permission on subscription) - it will be used in terraform [guide]([https://link](https://docs.microsoft.com/en-us/azure/active-directory/develop/howto-create-service-principal-portal))
5. Create the AKS cluster in Azure following instructions in Infra/Readme.md
6. Deploy web application and database by following instructions in AppDeploy/Readme.md
7. Test web application

