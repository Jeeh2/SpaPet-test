# README - Projeto SpaPetTest

## Participantes
Jessica de Oliveira Alves | Jessica Lima | Luciana Souza Ferreira de Oliveira

## Introdução
Este projeto consiste em testes end-to-end que são realizados diretamente no projeto disponível em https://github.com/lucianasfoliveira/SpaPetTest. O objetivo é garantir a integridade e funcionalidade da aplicação por meio de cenários de teste automatizados.

## Requisitos
O projeto requer a implementação de pelo menos 2 cenários de teste end-to-end. Esses cenários devem abranger a aplicação em todas as suas camadas, incluindo a conexão com o banco de dados. Utiliza-se Cucumber para a escrita dos cenários e Rest Assured para as requisições HTTP.

## Configuração do Ambiente
Certifique-se de ter o Java 11 ou 17 instalado em seu sistema.

## Funcionalidades
### Feature: Customer Login
#### Scenario: Customer tries to login with invalid email and password
Given an existing customer with invalid email and password

When the customer attempts to log in

Then the system returns a 403 Unauthorized status

#### Scenario: Validation of error message for invalid login
Given an existing customer with invalid email and password

When the customer attempts to log in

Then the system returns a 403 Unauthorized status

And the error message is displayed to the customer
