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
**Capex:** data-center tradicional (on-premises). \
**Opex:** AWS. \
Capex é a despesa de capital, Opex é uma despesa operacional. \ 

**Hypervisor:** virtualização de Sistemas Operacionais\
Arquiteturas tipo 1 (bare-metal) e tipo 2 (hosted).\

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

## Modelos de Computação em nuvem: IaaS, PaaS, SaaS.
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
	
## Free Tier AWS
Uma conta Free Tier é o conjunto de três tipos de ofertas: os do tipo **sempre gratuito**, os que **expiram em 12 meses** e os de **testes de curto prazo.**

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

## Documentação de Preços dos Produtos AWS
**Modo Convêncional:** ir na página do produto e clicar em "Definição de Preço".\
**Moro Rápido:** Alterar a URL do produto, exemplo: https://aws.amazon.com/pt/s3/pricing , aqui alteraríamos só o S3 por outro serviço, como por exemplo: https://aws.amazon.com/pt/ec2/pricing, sendo necessário conhecer o nome do serviço apenas.

## Calculadora AWS (pode não cair, só ler de vez em quando)
**Custo Simples Mensal (AWS Simple Monthly Calculator):** cobre todos os serviços aws utilizados e apresenta um custo estimado mensal.\
**Custo Total de Propriedade (AWS Total Cost of Ownership (TCO) Calculator:** comparar custo da execução de uma aplicação em ambiente local e em ambiente de nuvem aws.

## AWS Pricing Calculator (ESTUDAR mais essa!!!)
Link: https://calculator.aws/ \
A AWS Pricing Calculator é utilizada para estimar o curso dos produtos e serviços\
**1. Adicione o Serviço:** realize a busca pelo nome ou característica\
**2. Configure e Ajuste:** altere os detalhes de uso e o custo do serviço\
**3. Obtenha Estimativa:** custos separados por serviços, grupo ou total.

## AWS Organizations
**O que é o AWS Organizations?** \
É um serviço global que ajuda a administrar o seu ambiente em um único local.

**O que é um Organization Unit (OU)?** \
É um grupo de contas da AWS dentro de uma organização. \
Uma OU também pode conter oturas OUs, o que permite criar uma hierarquia.

**O que são Políticas de controle de serviço (SCPs)?** \
São políticas que definem ações do que usuários, grupos e funções do IAM podem realizar nas contas.

**Qual é o serviço utilizado para consolidar faturas?**
AWS Organizations

**Características:**
1. É um serviço global, 
2. Permite gerenciar múltiplas contas AWS, 
3. A conta principal é chamada de Master Account, 
4. As outras contas são chamadas de Member Account, 
5. Contas são organizadas por: Organizational Units (OU) 
6. Políticas de controle de serviço (Service Control Polices: SCP),
7. Consolida o pagamento de todas as contas em um único local.

## AWS Management Console & Aplicativo
São as maneiras de acessar a AWS. \
**Console de Gerenciamento (navegador):** é a interface grática acessada via navegador e pelo app em smartphone (AWS Console Mobile App) \
**Command Line Interface (CLI):** ferramente open source, conseguimos acesso ao root da instância, dá suporte a linux, macos, windows, powershell, ssh, etc \
**Software Development Kit (SDK):** API para acecssar a AWS através de nossos sistemas. \
**DICA PARA O EXAME:** \
- Existem três tipos de conexão: \
1. Console de Gerenciamento AWS (via https e app) 
2. AWS Command Line Interface (via terminal) 
3. Software Development Kit (via API, programação).

## AWS Identity and ACESS Management (IAM)\
Usuários: pessoas ou serviços, com credenciais **permanentes**.\
Grupos: Coletivo de usuários, grupos não podem conter outros grupos.\
Funções: não são suas permissões, é um método de autenteicação temporária (como um usuário temporário).\
![image](https://user-images.githubusercontent.com/74719360/166081290-12fdcfa3-8985-477b-85f4-4f1fddacccb7.png)\
**PARA A PROVA:**\
**Usuários** possuem credenciais **permanenetes** e **funções** possuem credenciais **temporárias**\
Usuários root **NÃO** devem ser compartilhados\
Use o **least privilege principle** nos usuários.\
Documentos **JSON** definem as **permissões** de acesso\
**Grupos** contém outros usuários, mas **não** podem **conter outros grupos**.

## AWS WAF
O **AWS WAF** é um firewall de aplicativos web que permite especificar qual tráfego é permitido ou bloquear, mediante a definição de regras personalizáveis.\
**Características:** \
Filtrar o tráfego com regras personalizadas \
Bloquear requisições como SQL Injection (SQLi), e cross-site scripting (XSS) \
Fácil ajuste e monitoramenteo do tráfego. \
![image](https://user-images.githubusercontent.com/74719360/166107906-640036df-204f-4458-a7f0-d688e9ccb5ac.png) \

## AWS Shield
O AWS Shield é um serviço gerenciado de proteção contra DDoS (negação de serviço distribuída) que protege os aplicativos executados na AWS. \
**Características:** \
Proteção contra DDoS \
Monitoramento de fluxo e tráfego de aplicativos \
Suporte 24x7 com especialistas \
A versão Standart é suficiente para quase todos os cenários. Caso deseje mais opções de configuração e relatórios detalhados, pode-se contratar o AWS Shield Advanced. \

## Amazon Cognito
Permite adicionar cadastramento, login e controle de acesso de usuários a aplicativos web e móveis, com o login do Facebook, Google, Amazon e de provedores de identidade empresariais. \
**Característica:** \
Federação de identidades sociais e empresariais \
Diretório de usuários seguro e escalável \
Autenticação baseada em padrões \
Segurança para aplicativos e usuários \
Controle de acesso para recursos da AWS \
Fácil integração com os aplicativos. 

## Criptografia na AWS
Criptografia é uma técnica de proteção aplicada ao dado em respouso [at rest] ou em trânsito [in transit], para não permitir o acesso ou a leitura de pessoas sem autorização. \

**Criptografia para objetos** \
**S**erver **S**ide **E**ncryption\ 
<br>
SSE-S3: objetos S3 e a AWS gerencia as chaves. \
SSE-KMS: utiliza o AWS Key Managment Service para gerenciar as chaves. \
SSE-C: você gerencia suas chaves. \
<br>
**Client Side Encryption** \
Criptografia antes de enviar ao S3, usando uma chave mestra CMK. \
**O QUE TER ATENÇÃO NO EXAME?** \
De quem é a responsabilidade da criptografia? R: você! \
Quais são os tipos de criptografia do lado do servidor? R: SSE-S3, SSE-KMS, SSE-C \
**Qual o serviço que gerencia a chave de criptografia? R: AWS KMS (Key Management Service)** \
Qual a chave para criptografia do lado do cliente? R: Customer Master Key (CMK), Chave Mestra do Cliente.

## Amazon EC2 - Elastic Compute Cloud
O Amazon EC2 é um serviço que disponibiliza uma capacidade computacional segura, representado por uma instância redimensionável na Nuvem. \
**Características:**
1. Amazon EC2 -> Elastic Compute Cloud
2. Modelo infraestrutura como Serviço\
3. Alugar máquinas virtuais (EC2)\
4. Armazenar dados em volumes virtuais (EBS) \
5. Distribuir a carga de trabalho (ELB) \
6. Escalar o serviço de acordo com a demanda (ASG)\
![image](https://user-images.githubusercontent.com/74719360/167248965-5ed98620-1c25-41f1-8204-06ae1c35ce81.png) \
![image](https://user-images.githubusercontent.com/74719360/167249030-b3d3b4e7-67ac-4cb9-a0b6-e37d457dafaa.png) \
**Lembre-se para a prova:** \
O **Amazon EC2** é um serviço web que disponibiliza uma c**apacidade computacional** segura, representado por uma **instância redimensionável** na Nuvem. \
**Modelo Computacional** é **Infraestrutura como Serviço** \
**Ambiente Operacional** tipo **Windows, MacOSe Linux** \
**Cobrança** por **hora** ou **segundo** (mínimo de 60 segundos) 

## Amazon EC2 - Launch Types (inicializadores)
São divididos em:
* **Sob demanda**  \
![image](https://user-images.githubusercontent.com/74719360/167249545-5849b947-618d-4f9c-be99-69fd76d6aec4.png)  \

* **Instâncias Spot** \
![image](https://user-images.githubusercontent.com/74719360/167249761-1e87d180-ee2d-4bcf-a64a-cfbc9ab0e164.png) \

* **Instâncias Reservadas** \
![image](https://user-images.githubusercontent.com/74719360/167249644-ddd5d408-faff-4a18-ae65-6a362fbea640.png)  \

* **Host e Instância Dedicada** \
![image](https://user-images.githubusercontent.com/74719360/167249710-e5b3807f-3d44-4191-918b-bb0ef523813e.png) \
![image](https://user-images.githubusercontent.com/74719360/167249751-efa721e4-b2f1-4245-ae56-81fc03435dc5.png) \
![image](https://user-images.githubusercontent.com/74719360/167249756-11dd5b8a-fea7-4906-8c5c-b061206a7a64.png) \

**Resumo para a prova** \
![image](https://user-images.githubusercontent.com/74719360/167249811-c7b3d06a-54f7-4ccc-acd2-2e7683a86295.png) \

## AWS Lambda
Permite que você execute códigos sem provisionar ou gerenciar servidores, pagando apenas pelo número de solicitações e pelo tempo de computação que você utilizar. \
<br>
**Características:**
* Serverless
* Escalável
* Baixo custo
* Multiplas linguagens
![image](https://user-images.githubusercontent.com/74719360/167317369-bd4bb9b3-cfe0-4258-90d9-7bbdb9e63f12.png)

Para a prova:
* Serviço serverless e gerenciado pela AWS
* AWS Lambda dimensiona suas aplicações
* Você pode otimizar o tempo de execução e o tamanho de memória (até 10GB)
* Cobrança por número de solicitações de suas funções e pela duração por cada milissegundo que leva para que seu código seja executado (até 15 minutos)

## AWS Elastic Beanstalk
É um serviço gerenciado, para os desenvolvedores realizarem uma fácil utilização de implantação e escalabilidade de aplicações e serviços web.\
![image](https://user-images.githubusercontent.com/74719360/167317743-e300af53-ff01-4103-aead-346f3b23b40d.png) 
![image](https://user-images.githubusercontent.com/74719360/167317899-82a3b0c2-6765-4ae4-90e6-7444ab92a51d.png)

## Amazon Lightsail
Uma plataforma na nuvem que oferece o que você precisa para criar um aplicativo ou um site, com um plano mensal de baixo custo. \
![image](https://user-images.githubusercontent.com/74719360/167318018-d2dd8f6e-23e0-4d5d-95e6-982f3dd947ae.png)
![image](https://user-images.githubusercontent.com/74719360/167318052-74634860-69cf-4c94-bcc2-46f6b61c5b6a.png)
![image](https://user-images.githubusercontent.com/74719360/167318072-89fa7227-0e49-4fd5-8d97-d4cbbe25ede0.png)
![image](https://user-images.githubusercontent.com/74719360/167318087-9948c8c1-ea71-4c77-9688-9d47add23451.png)

Para a prova: \
**Aplicações de Uso:**  
* Aplicativo web simples
* Software comercial e código aberto
* Site de blog, pessoal ou e-commerce
* Ambiente de testes e desenvolvimento
* Pagamento através de um plano mensal de baixo custo.

## Amazon S3 - Simple Storage Service
É um serviço gerenciado de armazenamento e recuperação de objetos, respondendo com escalabilidade, disponibilidade, segurança e performance.
**Benefícios do Amazon S3**
* Armazenamento virtualmente ilimitado
* Compartilhar arqvuiso ou criar um website estático
* Armazenar snapshops, backups, gerar um armazenamento híbrido do seu ambiente on-premises.
* Repositório de data lakes e análise de big data
* Baixa latência e alta velocidade
* Durabilidade de 99,999999999 (onze noves)

**Nomenclaturas**
* ARMAZENAMENTO = BUCKETS
* ARQUIVOS = OBJETOS
* SUB-PASTAS = PREFIXOS

