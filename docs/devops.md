# Docker, DevOps & Deployment

A curated guide to packaging, automating, and shipping .NET apps. For desktop tooling (Docker Desktop, CLIs), see [Tools](./tools.md).

## Containerizing .NET

1. [Containerize a .NET app — Tutorial](https://learn.microsoft.com/en-us/dotnet/core/docker/build-container)

	The official step-by-step for putting a .NET app in a Docker container.

2. [Build container images with the .NET SDK](https://learn.microsoft.com/en-us/dotnet/core/containers/sdk-publish)

	Produce an image with `dotnet publish --container` — no Dockerfile required.

3. [.NET Chiseled Containers](https://devblogs.microsoft.com/dotnet/announcing-dotnet-chiseled-containers/)

	Ultra-small, hardened base images with no shell or package manager — smaller and more secure.

4. [.NET Docker Samples](https://github.com/dotnet/dotnet-docker/tree/main/samples)

	Official sample Dockerfiles — multi-stage builds, Alpine, and best practices.

## CI/CD

1. [Building and testing .NET — GitHub Actions](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-net)

	Official guide to building, testing, and publishing .NET in GitHub Actions.

2. [actions/setup-dotnet](https://github.com/actions/setup-dotnet)

	The official Action to install and cache the .NET SDK in your workflows.

3. [Build .NET apps with Azure Pipelines](https://learn.microsoft.com/en-us/azure/devops/pipelines/ecosystems/dotnet-core)

	Set up CI/CD for .NET on Azure DevOps Pipelines.

## Orchestration & Hosting

1. [.NET Aspire](https://learn.microsoft.com/en-us/dotnet/aspire/)

	Microsoft's stack for orchestrating multi-service .NET apps locally and in the cloud.

2. [Kubernetes Documentation](https://kubernetes.io/docs/home/)

	The reference for deploying and scaling containerized apps in production.

3. [Deploy ASP.NET Core to Azure App Service](https://learn.microsoft.com/en-us/azure/app-service/quickstart-dotnetcore)

	The fastest managed way to host a .NET web app on Azure.

4. [.NET on AWS](https://aws.amazon.com/developer/language/net/)

	SDKs, tooling, and deployment paths for running .NET on AWS.

5. [Railway](https://railway.app/) · [Render](https://render.com/) · [Fly.io](https://fly.io/)

	Developer-friendly platforms for deploying containerized .NET apps with minimal setup.
