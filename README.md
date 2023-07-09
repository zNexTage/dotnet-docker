## Dotnet Docker

Exemplo de como configurar o Docker para rodar uma aplicação .NET Core 7.
Toda a configuração do Docker está em `Dockerfile`.

# 1. Comandos necessários
- Montando a imagem: `docker build --rm -t dotnetdocker:latest .`;
- Rodando o contâiner: `docker run --rm -p 5000:5000 -p 5001:5001 -e ASPNETCORE_HTTP_PORT=https://+:5001 -e ASPNETCORE_URLS=http://+:5000 dotnetdocker`
- Acesse: `localhost:5000/WeatherForecast` para verificar que a aplicação está rodando.