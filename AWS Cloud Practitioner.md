# AWS Cloud Practitioner

##  Benefícios da Nuvem AWS
> Performance\
Disponibilidade\
Segurança\
Escalabilidade\
Confiança\
Baixo custo.

## O que é computação em nuvem?
É a entrega sob demanda de recursos computacionais, por meio de uma plataforma de serviços via internet, sem gerenciamento ativo do usuário.

## Capex vs. Opex
**Capex:** data-center tradicional (on-premises).
**Opex:** AWS.
Capex é a despesa de capital, Opex é uma despesa operacional. 

**Hypervisor:** virtualização de Sistemas Operacionais
Arquiteturas tipo 1 (bare-metal) e tipo 2 (hosted).

Bare Metal, tipo 1\
VM - Guest OS	VM - Guest OS\
HyperVisor\
Hardware

Hosted, tipo 2\
VM - Guest OS	VM - Guest OS\
HyperVisor\
Host OS\
Hardware

## Seis vantagens da computação em nuvem
**Save Money:** pagar somente pelos recursos consumidos, ao invés de investir em infraestrutura on-premises.\
**Stop guessing:** não é necessário adivinhar quanto de hardware você irá utilizar.\
**Variable Expenses:** pagar apenas o que consumir.\
**Economies of scale:** quanto mais empresas utilizarem o AWS, menor será o custo para todos.\
**Increase speed and agility:** upgrade ao passo de alguns clicks.\
**Go global:** sua aplicação em várias regiões do mundo com apenas alguns clicks.

## Modelos de Computação tradicional: IaaS, PaaS, SaaS.
**IaaS:** infraestrutura como serviço. Hospedagem comum, hostgator, hostinger, etc.\
**PaaS:** plataforma como serviço. A plataforma faz tudo, você foca no desenvolvimento.\
**SaaS:** software como serviço. Você só se preocupa em como executar o software, ex.: gmail.

## Modelos de Implantação
**On-premises (nuvem privada):** recursos dedicados.\
**Hybrid:** sua infra on-premises e nuvem juntas.\
**Cloud:** tudo na nuvem.

## Escalabilidade, Elasticidade e Alta Disponibilidade
#### Escalabilidade e Alta Disponibilidade
Existem dois tipos de escalabilidade: Vertical e Horizontal (também conhecido como: (elasticidade).

**Escalabilidade Vertical:** aumentar o poder computacional da instância\
Ex.:\
T2.Micro com 1 vCPU e 1GB RAM -> T2.Large com 2vCPU e 8GB RAM.

**Escalabilidade Horizontal:** aumentar a quantidade de instâncias que rodam a aplicação.\
Ex.:\
De 01 t2.micro em execução para 10 t2.micro em execução.

**Alta Disponibilidade:** anda de mãos dadas com a escalabilidade horizontal, na alta disponibilidade, você roda sua aplicação em pelo menos duas zonas de disponibilidade. O nome dessa estratégia se chama Disaster Recovery (DR), na AWS disponibilizamos nossas instâncias em duas ou mais zonas de disponibilidade, em caso de uma sofrer algum incidente, o negócio não é afetado.

**RESUMO:**
Escalabilidade Vertical = aumentar poder computacional.\
scale up -> aumentar & scale down -> diminuir.\
Escalabilidade Horizontal = aumentar a quantidade de instâncias.\
scale out -> aumentar & scale in -> diminuir.\
Alta disponibilidade = instâncias em diferentes zonas de disponibilidade, estratégia de Disaster Recovery (DR).

## Política de uso aceitável: regras do que pode ou não fazer na AWS.
>	Nenhum uso ou conteúdo ilegal, prejudicial ou ofensivo.\
	Nenhuma violação de segurança.\
	Nenhum abuso de rede.\
	Nenhum abuso de e-mail ou outras mensagens (ex.: spam). 

## AWS Serverless
É criar e executar aplicações sem se preocupar com servidores. Serverless não significa que não existem servidores, mas sim que eles existem, mas não os gerenciamos. Ex.: AWS Lambda, AWS Fargate, Amazon EventBridge etc.

## Regiões, Zonas de Disponibilidade e Pontos de Presença
Uma **REGIÃO** é a disponibilização de uma coleção de recursos AWS em uma localização geográfica, sendo ele composto por um conjunto de zonas de disponibilidade.
Uma região é um conjunto de zonas de disponibilidade [Região(Zonas de Disp)]

Uma **ZONA DE DISPONIBILIDADE** é um ou mais data centers que estão na mesma **REGIÃO**, porém separados a quilômetros de distância, com energia, rede e conectividade redundantes. [Região(Zonas de Disponibilidade: data centers)]

Um **PONTO DE PRESENÇA** é uma infraestrutura de servidores, localizado próximo de uma Zona de Disponibilidade, que armazena os dados mais solicitados no cache, para entrega com menor latência uma requisição de consulta.
 
## Responsabilidade Compartilhada

Enquanto a AWS gerencia a segurança da nuvem, a segurança na nuvem é de responsabilidade do cliente. Os clientes mantêm o controle de qual segurança eles escolhem implementar para proteger seu próprio conteúdo, plataforma, aplicativos, sistemas e redes, da mesma forma que em um datacenter no local.

## Auditoria AWS
A AWS é continuamente auditada, obtendo certificações em todas as regiões geográficas em que ela está disponível.
Os relatórios de conformidade (compliance) e os acordos de uso de serviços (agreements), são armazenados no serviço AWS Artifact.

## Recursos Gerenciados x Recursos não gerenciados
Um recurso gerenciado é quando um serviço ou algumas configurações da camada anterior de configuração não é administrada pelo usuário, ao passo que se esse serviço ou configuração seja administrada pelo usuário, temos um recurso não gerenciado.

## Estado de Saúde dos Serviços AWS
Serve para ver a “saúde” dos serviços AWS, ou seja, sua disponibilidade e status normal ou irregular. 

## AWS Personal Health Dashboard 
É o serviço que apresenta os alertas e notificações do ambiente e serviços da AWS, como falhas por exemplo.

## AWS Budget
Orçamento e aviso de orçamento AWS.

## Serviços AWS
Um produto AWS é o coletivo de serviços, possuindo propósitos e características individuais, para ajudar cliente em ir rapidamente para a Nuvem, baixar os custos de TI e simplificar na escalabilidade.
[Produto(Serviços:propósito e características)]
Na prova cai 12 produtos da AWS, temos que DECORAR:
> Análise\
Banco de Dados\
Armazenamento\
Computação\
Gerenciamento e Governança\
Integração de Aplicações\
Computação sem servidor\
Redes e entrega de conteúdo\
Segurança, identidade e conformidade\
Gerenciamento financeiro na nuvem\
Ferramentas do desenvolvedor\
Migração e transferência.


