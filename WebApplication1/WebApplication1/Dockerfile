FROM microsoft/aspnetcore:1.1



COPY . /app
WORKDIR /app

RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]

EXPOSE 80/tcp
ENV ASPNETCORE_URLS http://*:80

ENTRYPOINT ["dotnet", "run"]
