TechStore - Arquitetura de Infraestrutura em Nuvem

Objetivo

Documentar uma arquitetura de infraestrutura em nuvem para uma empresa fictícia chamada TechStore, utilizando serviços da Amazon Web Services (AWS).

Serviços AWS utilizados

Amazon VPC: rede virtual
Amazon EC2: servidor de aplicação
Amazon RDS: banco de dados relacional
Amazon S3: armazenamento de arquivos
AWS IAM: gerenciamento de permissoes
Elastic Load Balancing: Distribuição de tráfego
Amazon CloudWatch: Monitoramento

Segurança

Security Groups: controla tráfego de rede
IAM: para controlar acessos e permissões
Principios: do menor privilégio
Separação: entre aplicação e banco de dados

Implementação

Projeto desenvolvido em ambiente Ubuntu no WSL 2, com documentação e organização utilizando Git.

A arquitetura é uma simulação conceitual. Nenhum recurso real foi implantado na AWS.

Tecnologias e ferramentas

Ubuntu
WSL 2
Git
GitHub
AWS (Arquitetura Conceitual)

Autor

Lucas Pereira Bello
## Banco de Dados MySQL

O projeto também possui uma implementação prática de banco de dados relacional utilizando MySQL 8.4 no Ubuntu Linux (WSL2).

### Atividades realizadas
- Criação do banco de dados TechStore.
- Criação de tabelas e relacionamentos.
- Inserção e consulta de dados.
- Consultas SQL com INNER JOIN.
- Atualização e análise de estoque.
- Criação de VIEW e INDEX.
- Geração de backup com mysqldump.

### Evidências
As capturas de tela das atividades estão disponíveis na pasta `evidencias/`.

### Backup
O backup do banco está em `scripts/techstore.sql`.
