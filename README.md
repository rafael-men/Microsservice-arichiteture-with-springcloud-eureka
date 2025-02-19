# Microsserviços Java Spring Boot com Archaius, Eureka e Load Balancer

## 📌 Descrição
Este projeto implementa uma arquitetura baseada em **microsserviços**, utilizando:

- **Netflix Archaius** para gerenciamento dinâmico de configurações.
- **Netflix Eureka** para descoberta de serviços.
- **Spring Cloud LoadBalancer** para balanceamento de carga entre as instâncias dos serviços.

## ⚙️ Tecnologias Utilizadas

- **Spring Boot**
- **Netflix Archaius**
- **Netflix Eureka**
- **Spring Cloud LoadBalancer**
- **Maven**
- **Docker e Docker Compose** (para facilitar a execução dos serviços)

## ✅ Pré-requisitos

Antes de executar a aplicação, certifique-se de ter instalado:

- **Java 8** ou superior
- **Maven 3.6.0** ou superior
- **Docker** e **Docker Compose**

## 🛠️ Como funciona o Eureka?

O **Eureka Server** atua como um **registro de serviços**, permitindo que os microsserviços se registrem e descubram uns aos outros dinamicamente.

1. O **Eureka Server** deve estar em execução antes de iniciar os microsserviços.
2. Os serviços clientes (microsserviços) se registram automaticamente no Eureka Server.
3. O balanceador de carga usa o Eureka para rotear chamadas entre as instâncias disponíveis.

## 🚀 Como executar com Docker Compose


Crie um arquivo `docker-compose.yml` na raiz do projeto:

## 🏃‍♂️ Rodando a aplicação

Clone o repositório:


git clone https://github.com/seu-repositorio/microsservicos-eureka.git
cd microsservicos-eureka

Construa as imagens dos serviços:

docker-compose build

Inicie os containers:

docker-compose up -d

Acesse o Eureka Server no navegador:

http://localhost:8761

Teste os microsserviços acessando o endpoint do API Gateway
