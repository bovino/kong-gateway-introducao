# Introdução ao Kong API Gateway
Repositório com ambiente de exemplo para rodar o Kong 2.8.1 DBLESS localmente usando o docker compose (apresentação feita para o Brazil Online Meetup da Kong de Junho de 2022)

## Instruções de uso

- Instale o Docker Engine (alguma versão que suporte o Docker Compose)
- Clone este repositório
- Na pasta raiz rode ` docker-compose up` (certifique-se de que estão livres as portas 8000, 8001, )
- Sorria e dispare requisições para algumas rotas ( GET http://localhost:8000/v1/my-plugin-data or POST http://localhost:8000/v3/my-plugin-data)
- Para parar de rodar voce pode rodar ` docker-compose down` e ` docker-compose kill`
- Para ver como rodar um ambiente Kong localmente preparado para o desenvolvimento de plugins customizados use este outro reposítório aqui (https://github.com/bovino/kong-template-with-docker)
- Tenha em mente que este é um setup visando estudos e aprendizado, não sendo um setup indicado para ambientes produtivos, para ver uma referência de ambiente com características adicionais de robustez e segurança você pode olhar este repositório aqui (https://github.com/Kong/docker-kong/tree/master/compose)
- Na pasta "insomnia" há um projeto de exemplo que você pode importar no seu ambiente Insomnia já contendo chamadas configuradas para os endpoints e para a Admin API do Kong