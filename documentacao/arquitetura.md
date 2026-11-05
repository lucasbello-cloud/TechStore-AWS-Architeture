
Arquitetura de Infraestrutura AWS - TechStore

Visão Geral

A TechStore é uma empresa fictícia de comércio eletrônico que precisa de uma infraestrutura em nuvem para hospedar sua aplicação, armazenar arquivos e gerenciar dados com segurança.

A arquitetura utiliza serviços da AWS para organizar os componentes da solução.

Componentes de Infraestrutura

VPC: rede virtual isolada
Subnets Públicas: destinada aos componentes que precisam
Subnets Privadas: destinadas aos recursos internos
Internet Gateway: permite comunicação entre a VPC e a Internet
EC2: servidor responsavel pela aplicação
RDS: banco de dados relacional
S3: armazenamento de arquivos
Security Groups: controla o tráfego de banco de dados

Fluxo de funcionamento

Fluxo de funcionamento

1. O usuário acessa a aplicação pela internet.
2. O tráfego é direcionado ao Load Balancer.
3. O Load Balancer encaminha as solicitações ao servidor EC2.
4. A aplicação EC2 consulta os dados armazenados no RDS.
5. Os arquivos são armazenados no Amazon S3.
6. O CloudWatch monitora o funcionamento dos recursos.

## 4. Organização da rede

A VPC representa a rede virtual principal da infraestrutura.

Ela é dividida em subnets públicas e privadas.

- A subnet pública permite acesso aos componentes que precisam receber tráfego externo.
- A subnet privada mantém recursos internos protegidos.
- O Internet Gateway conecta a VPC à internet.
- Os Security Groups controlam quais conexões são permitidas

## 5. Segurança e monitoramento

- IAM: gerenciamento de usuários e permissões.
- Security Groups: controle de tráfego.
- Menor privilégio: conceder somente as permissões necessárias.
- CloudWatch: monitoramento de métricas e eventos.

## 6. Observação

Esta arquitetura é um projeto de estudo e simulação conceitual. Os serviços AWS foram documentados, mas não foram implantados em uma conta real.

