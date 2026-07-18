FROM mcr.microsoft.com/dotnet/sdk:8.0

WORKDIR /source

COPY . .
RUN dotnet restore "OLX.API/OLX.API.csproj"

WORKDIR /source/OLX.API
RUN dotnet publish -o /app
WORKDIR /app

ENTRYPOINT ["dotnet", "OLX.API.dll"] 

