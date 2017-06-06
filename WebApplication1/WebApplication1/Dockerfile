FROM microsoft/aspnetcore:1.1

#RUN ["dotnet", "restore ./WebApplication1.sln"]
#RUN ["dotnet", "publish ./WebApplication1.sln -c Release -o ./obj/Docker/publish"]

ARG source
WORKDIR /app
EXPOSE 80
COPY ${source:-obj/Docker/publish} .



#ENTRYPOINT ["dotnet", "WebApplication1.dll"]
ENTRYPOINT ["dotnet", "run"]
