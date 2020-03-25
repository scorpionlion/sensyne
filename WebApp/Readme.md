[Sample Application](https://docs.docker.com/compose/aspnet-mssql-compose/)

1. Open bash command line in current directory 

2. Run below command


`
docker run -v ${PWD}:/app --workdir /app microsoft/dotnet:2.1-sdk dotnet new mvc --auth Individual
`

