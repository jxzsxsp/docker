FROM openchain_openchain

RUN mkdir -p /openchain/data

COPY config.json /openchain/data/config.json

WORKDIR /openchain

EXPOSE 8080
ENTRYPOINT ["dotnet", "openchain.dll"]
