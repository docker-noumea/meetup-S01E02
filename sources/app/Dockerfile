FROM microsoft/dotnet:latest
 
ENV ASPNETCORE_ENVIRONMENT="Production"
 
COPY . /app
WORKDIR /app
RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]
 
EXPOSE 5000/tcp
ENTRYPOINT ["dotnet", "run"]
