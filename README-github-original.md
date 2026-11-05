TechStore – Arquitetura em Nuvem AWS

 Objetivo

Representar a infraestrutura de uma loja virtual fictícia utilizando serviços da Amazon Web Services (AWS).

 Serviços utilizados

 VPC: rede virtual privada.
 Internet Gateway: comunicação com a internet.
 Application Load Balancer: distribuição de tráfego.
 EC2: servidores de aplicação.
 RDS: banco de dados.
 S3: armazenamento de arquivos.
 NAT Gateway: acesso à internet pelas sub-redes privadas.
 IAM: controle de permissões.
 CloudWatch: monitoramento.
 Security Groups: regras de acesso à rede.

 Arquitetura

Diagrama de Arquitetura

A infraestrutura utiliza duas Zonas de Disponibilidade, com sub-redes públicas e privadas.

4. Objetivo da arquitetura

Organizar os serviços da loja virtual, distribuir o tráfego, armazenar dados e arquivos e melhorar a disponibilidade e a segurança.



 Funcionamento da arquitetura

 O usuário acessa a loja virtual pela internet.
 O Internet Gateway permite a comunicação com a internet.
 O Application Load Balancer recebe as solicitações e distribui o tráfego entre os servidores EC2.
 Os servidores EC2 processam as solicitações.
 O Amazon RDS armazena os dados da aplicação.
 O Amazon S3 armazena arquivos.
 O NAT Gateway permite que as instâncias privadas iniciem conexões com a internet.
 O IAM controla as permissões e o CloudWatch monitora os recursos.


 Segurança da arquitetura

A segurança da infraestrutura é organizada por meio de:

 AWS IAM: controla usuários, funções e permissões.
 Security Groups: controlam o tráfego de entrada e saída dos recursos.
 Sub-redes privadas: mantêm os servidores e o banco de dados sem exposição direta à internet.
 NAT Gateway: permite acesso de saída à internet pelas sub-redes privadas.

 Monitoramento

O Amazon CloudWatch acompanha o funcionamento dos recursos da infraestrutura, permitindo observar métricas e identificar possíveis problemas.

Alta disponibilidade do banco de dados

O Amazon RDS utiliza a configuração Multi-AZ, com uma instância principal e uma réplica em espera em outra Zona de Disponibilidade.

Essa configuração ajuda a manter o banco de dados disponível caso ocorra uma falha na zona principal.


 Conclusão

O projeto TechStore demonstra como uma loja virtual pode utilizar serviços da AWS para organizar sua infraestrutura em nuvem.

A arquitetura apresenta distribuição de tráfego, servidores de aplicação, banco de dados, armazenamento de arquivos, controle de acesso e monitoramento.

Este projeto foi desenvolvido como estudo prático de Computação em Nuvem, utilizando uma arquitetura representativa da AWS.


 Competências desenvolvidas

 Arquitetura de infraestrutura em nuvem AWS.
 Redes virtuais e sub-redes.
 Alta disponibilidade com Multi-AZ.
 Balanceamento de carga.
 Armazenamento em nuvem.
 Segurança e controle de acesso.
 Monitoramento de infraestrutura.

 Observação

Este é um projeto educacional e conceitual. A infraestrutura foi representada em um diagrama, sem implantação de recursos reais na AWS.
