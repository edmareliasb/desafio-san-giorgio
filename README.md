# Visão Geral da Solução

Aqui está sendo descrito a solução tecnica de um desafio da compass uol

## Arquitetura

![Arquitetura drawio](https://github.com/user-attachments/assets/19ff0e1d-1f87-4485-8893-dd1312f94821)

## Stack de tecnologias
- Java 21
- Spring Boot 3.3.0
- AWS SDK
- Testes unitario
- Mockito
- Localstack
- Junit
- Banco de Dados
- Postgresql
- Redis

## Banco de Dados

Modelagem das Tabelas do Banco do Dados Relacional Postgresql

![ModelagemBD drawio](https://github.com/user-attachments/assets/bbb458f0-df4b-43bd-8803-cc4874a3c5f4)

## Swagger API de Validação de Pagamentos
Segue o swagger com a especificação de como deve ser implementado a api de validação de pagamentos.

Observação: Arquivo openapi.yaml completo encontra-se no repositorio

Assinatura da API com os parametros de requisção

![swagger-1](https://github.com/user-attachments/assets/8cfd279c-bf5b-4013-abb6-408869e04ef0)

Segue o Response body da API

![swagger-2](https://github.com/user-attachments/assets/5f19d14d-58c1-48a8-aa6a-9428706ab067)

## Payload SNS AWS
Segue o payload em formato JSON de como as mensagens serão enviadas para o topico payment_topic SNS da AWS.

Baseado no atributo paymentStatus do header da mensagem o serviço do SNS irá realizar o envio para a fila SQS correta.

![paymentTopicPayload drawio](https://github.com/user-attachments/assets/6415d69c-fa2c-435d-bb10-8664fca35006)

## Modelo de classes 
Segue o modelo de classes da soluçao seguinteo design Clean Architecture 

![Modelo de Classes drawio](https://github.com/user-attachments/assets/0d69344f-a0f1-4a97-8de4-d9c650ecee0d)

![Modelo de Classes_2 drawio](https://github.com/user-attachments/assets/1ddee0eb-9cb3-4ce6-b55d-9a78b38faec7)



