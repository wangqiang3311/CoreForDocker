FROM mcr.microsoft.com/dotnet/core/sdk:3.1
WORKDIR /app
COPY /. /app
RUN dotnet restore
RUN dotnet publish -o /out -c Release
EXPOSE 5000
ENTRYPOINT ["dotnet", "/out/CoreForDocker.dll"]