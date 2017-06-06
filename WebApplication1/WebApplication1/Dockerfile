FROM microsoft/aspnetcore:1.1

#RUN ["dotnet", "restore ./WebApplication1.sln"]
#RUN ["dotnet", "publish ./WebApplication1.sln -c Release -o ./obj/Docker/publish"]

ARG source=master
WORKDIR /app
EXPOSE 80
COPY master:-obj/Docker/publish .
ENTRYPOINT ["dotnet", "WebApplication1.dll"]
