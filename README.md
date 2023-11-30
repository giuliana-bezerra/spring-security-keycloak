<h1 align="center">
  Spring Security + Keycloak
</h1>

<p align="center">
 <img src="https://img.shields.io/static/v1?label=Youtube&message=@giulianabezerra&color=8257E5&labelColor=000000" alt="@giulianabezerra" />
 <img src="https://img.shields.io/static/v1?label=Tipo&message=Tutorial&color=8257E5&labelColor=000000" alt="Tutorial" />
</p>

Projeto apresentado [nesse vídeo](https://youtu.be/vV2NdanynpA) que ilustra o uso do Keycloak com Spring Security utilizando o Oauth 2.0 + OpenID.

## Configuração do Keycloak

1 - Executar Keycloak
```
docker run -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:22.0.5 start-dev
```

2 - Criar usuário e client oauth no Keycloak

## Testando a Aplicação

As seguintes rotas podem ser acessadas para testar:

- GET /public: Rota aberta
- GET /private: Rota que pede autenticação
- GET /cookie: Rota que pede autenticação com cookie de sessão
- GET /jwt: Rota que pede autenticação com JWT