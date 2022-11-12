#See https://aka.ms/containerfastmode to understand how Visual Studio uses this Dockerfile to build your images for faster debugging.

FROM mcr.microsoft.com/dotnet/aspnet:6.0 AS base
WORKDIR /app
COPY . .
EXPOSE 80
ENTRYPOINT ["dotnet", "sqlapp.dll"]

#FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build
#WORKDIR /src
#COPY ["sqlapp/sqlapp.csproj", "sqlapp/"]
#RUN dotnet restore "sqlapp/sqlapp.csproj"
#COPY . .
#WORKDIR "/src/sqlapp"
#RUN dotnet build "sqlapp.csproj" -c Release -o /app/build
#
#FROM build AS publish
#RUN dotnet publish "sqlapp.csproj" -c Release -o /app/publish
#
#FROM base AS final
#WORKDIR /app
#COPY --from=publish /app/publish .
#ENTRYPOINT ["dotnet", "sqlapp.dll"]
