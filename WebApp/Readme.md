[Sample Application](https://docs.docker.com/compose/aspnet-mssql-compose/)

1. Open bash command line in current directory 

2. Run command to download the sample and create app 
`
docker run -v ${PWD}:/app --workdir /app microsoft/dotnet:2.1-sdk dotnet new mvc --auth Individual
`

3. Build the app
`
docker-comppose build
`

4. Host and Test app locally
`
docker-comppose up
`

