# Diagrama da Arquitetura AWS - TechStore

## Arquitetura da infraestrutura

```mermaid
flowchart TD
    A[Usuário] --> B[Internet]
    B --> C[Load Balancer]
    C --> D[VPC]
    D --> E[EC2 - Aplicação]
    E --> F[RDS - Banco de Dados]
    E --> G[S3 - Arquivos]
    E --> H[CloudWatch - Monitoramento]
    I[IAM - Permissões] --> E
    J[Security Groups] --> D


Esse diagrama representa a arquitetura proposta, não uma implantação real.

Me avise quando terminar. Ainda não salve.
