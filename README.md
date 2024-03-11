<h1>Api de gestão de ingressos</h1>

Fluxograma responsavel pela a estrura de um software responsavel por venda de ingressos de shows de grande porte.

![Fluxo api de ingressos](https://github.com/Gabopontes/Api-de-gest-o-de-ingressos/assets/99334150/150e1366-d2ac-47dd-88c0-384688a472c8)


## Fluxo 
Usuário inicia sessão/compra → Servidores Web lidam com autenticação → Solicitações autenticadas encaminhadas ao Serviço de Inventário de Ingressos → Verificação em tempo real da disponibilidade de ingressos → Confirmação da compra ou enfileiramento durante períodos de alta demanda → Atualizações periódicas da disponibilidade de ingressos são comunicadas à Interface do Usuário.

## Técnologias que podem ser utilizadas

API de Login e Interface:
* ASP.NET Core (C#)
* Angular 
* Autenticação: Iautenticação local usando Identity no ASP.NET Core para lidar com o login. Serviços de login externos, como o Google, usando o protocolo OAuth.

Serviço de Inventário de Ingressos:
 * ASP.NET Core (C#)
 * Entity Framework e Dapper para interagir com o banco de dados de maneira eficiente.

Banco de Dados:
 * SQL Server.

Comunicação entre Componentes:
 * Protocolo de Comunicação: HTTP/HTTPS para a comunicação entre a API de Login, o Serviço de Inventário de Ingressos e outros componentes.

