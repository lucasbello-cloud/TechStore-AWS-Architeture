# Plano de Rede — TechStore AWS

## 1. Objetivo
Definir a organização das redes da infraestrutura TechStore na AWS.

## 2. VPC
- Nome: TechStore-VPC
- CIDR: 10.0.0.0/16
- Região: us-east-1

## 3. Sub-redes

| Sub-rede | CIDR | Tipo |
|---|---|---|
| Public-A | 10.0.1.0/24 | Pública |
| Public-B | 10.0.2.0/24 | Pública |
| Private-App-A | 10.0.11.0/24 | Privada |
| Private-App-B | 10.0.12.0/24 | Privada |
| Private-DB-A | 10.0.21.0/24 | Privada |
| Private-DB-B | 10.0.22.0/24 | Privada |

## 4. Roteamento
- Rede pública: Internet Gateway.
- Aplicação: NAT Gateway.
- Banco de dados: sem acesso direto à internet.
- Comunicação interna: rota local da VPC.

## 5. Segurança
- Load Balancer: portas 80 e 443.
- EC2: acesso pelo Load Balancer.
- RDS: acesso pela aplicação.
- S3: acesso controlado por permissões.

## 6. Alta disponibilidade
A arquitetura utiliza duas zonas de disponibilidade.

## 7. Observação
Projeto conceitual para estudo. Nenhum recurso foi implantado na AWS.
