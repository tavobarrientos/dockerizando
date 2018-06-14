FROM microsoft/aspnetcore-build:2.0.0
COPY . /app
WORKDIR /app
RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]
 
ENV ASPNETCORE_URLS http://+:5000
EXPOSE 5000

ENTRYPOINT dotnet run