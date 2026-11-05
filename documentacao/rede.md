# Configuração de Rede - TechStore

## 1. VPC

A VPC (Virtual Private Cloud) é uma rede virtual isolada na AWS.

Ela permite organizar os recursos da infraestrutura dentro de uma rede controlada.

## 2. Subnets

As subnets dividem a VPC em redes menores.

- **Subnet pública:** utilizada por recursos que precisam de acesso externo.
- **Subnet privada:** utilizada por recursos internos, como o banco de dados.

## 3. Internet Gateway

O Internet Gateway (IGW) permite a comunicação entre a VPC e a internet.

Ele é associado à VPC e utilizado pelas rotas das subnets públicas.

## 4. Tabela de rotas

A tabela de rotas define para onde o tráfego de rede deve ser encaminhado.

- **Rota local:** permite comunicação dentro da VPC.
- **Rota para o Internet Gateway:** permite acesso à internet pela subnet pública.
- **Subnets privadas:** não recebem rota direta para o Internet Gateway.

## 5. Security Groups

Os Security Groups funcionam como firewalls virtuais associados aos recursos da AWS.

Eles controlam o tráfego de entrada e saída.

- EC2: permite somente as conexões necessárias à aplicação.
- RDS: permite acesso apenas a partir da aplicação autorizada.
- Aplicação: deve evitar exposição desnecessária de portas.

## 6. Resumo

A infraestrutura de rede da TechStore utiliza VPC, subnets públicas e privadas, Internet Gateway, tabelas de rotas e Security Groups.

O objetivo é organizar a comunicação entre os recursos e controlar o acesso à infraestrutura.
