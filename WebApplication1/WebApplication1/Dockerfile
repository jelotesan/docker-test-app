FROM microsoft/aspnetcore:1.1

#RUN ["dotnet", "restore ./WebApplication1.sln"]
#RUN ["dotnet", "publish ./WebApplication1.sln -c Release -o ./obj/Docker/publish"]

ARG Source
WORKDIR /app
EXPOSE 80
COPY ${Source:-obj/Docker/publish} .
ENTRYPOINT ["dotnet", "WebApplication1.dll"]
