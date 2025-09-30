# Dotnet 9 Blazor Web App

This project is a Blazor web application built with .NET 9.

## Workflow for Azure Deployment

### Environments

- **Production**
- **Staging**

### Steps

1. **Build the Application**
    ```bash
    dotnet build
    ```

2. **Run Locally**
    ```bash
    dotnet run
    ```

3. **Publish for Azure**
    ```bash
    dotnet publish -c Release -o ./publish
    ```

4. **Deploy to Azure**
    - Use Azure Portal or Azure CLI to deploy the contents of the `./publish` folder.
    - For staging, configure a separate deployment slot in Azure App Service.

## Useful Links

- [Blazor Documentation](https://learn.microsoft.com/en-us/aspnet/core/blazor/)
- [Azure App Service Deployment](https://learn.microsoft.com/en-us/azure/app-service/quickstart-dotnetcore?tabs=net80&pivots=development-environment-vs)

## Notes

- Ensure your Azure App Service is configured for .NET 9.
- Use environment variables to manage configuration between production and staging.
- Monitor deployments using Azure Application Insights.
