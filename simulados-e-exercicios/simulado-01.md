# Simulado 01: Visão Geral dos 4 Domínios (CLF-C02)

> Questões **originais**, escritas com base no guia oficial do exame e na documentação da AWS. Material independente, não afiliado à AWS.

| Item | Detalhe |
|---|---|
| Questões | 30 |
| Tempo sugerido | 40 minutos |
| Formato | Múltipla escolha e múltipla resposta (2 questões pedem duas respostas) |
| Meta | 80% ou mais (24 acertos) |

### Distribuição por domínio

| Domínio | Questões |
|---|:---:|
| 1. Conceitos de Nuvem | 1 a 7 |
| 2. Segurança e Conformidade | 8 a 16 |
| 3. Tecnologia e Serviços da Nuvem | 17 a 26 |
| 4. Cobrança, Preços e Suporte | 27 a 30 |

### Como fazer

1. Responda sem consultar nada, cronometrando o tempo.
2. Anote suas respostas antes de abrir os gabaritos.
3. Abra cada gabarito clicando em **Ver resposta**. Leia também o motivo de as outras alternativas estarem erradas, é onde está o aprendizado.
4. Ao final, use a tabela de resultado para saber o que revisar.

---

## Domínio 1: Conceitos de Nuvem

### Questão 1

Uma loja virtual recebe 20 vezes mais acessos durante a Black Friday e quer que a capacidade aumente e diminua automaticamente conforme a demanda. Qual vantagem da nuvem atende a esse cenário?

- A) Economia de escala
- B) Elasticidade
- C) Alcance global em minutos
- D) Alta disponibilidade

<details>
<summary>Ver resposta</summary>

**Resposta: B**

Elasticidade é a capacidade de aumentar e reduzir recursos conforme a demanda, pagando só pelo que usa.

- A) Economia de escala é o preço menor que a AWS consegue por agregar o uso de muitos clientes.
- C) Alcance global trata de implantar em várias Regiões rapidamente, não de ajustar capacidade.
- D) Alta disponibilidade trata de manter o serviço no ar diante de falhas.
</details>

### Questão 2

Qual descrição corresponde a uma **Zona de Disponibilidade (AZ)**?

- A) Um ponto de presença usado para cache de conteúdo
- B) Uma conta separada dentro do AWS Organizations
- C) Um ou mais data centers isolados dentro de uma Região, com energia e rede redundantes
- D) Uma conexão dedicada entre o cliente e a AWS

<details>
<summary>Ver resposta</summary>

**Resposta: C**

Cada Região tem várias AZs, isoladas entre si para que uma falha em uma não afete as outras.

- A) Isso descreve uma Edge Location.
- B) Contas pertencem ao AWS Organizations e não têm relação com infraestrutura física.
- D) Isso descreve o AWS Direct Connect.
</details>

### Questão 3

Uma equipe quer avaliar suas cargas de trabalho para reduzir o consumo de energia e o impacto ambiental. Qual pilar do **Well-Architected Framework** é o mais relacionado?

- A) Excelência Operacional
- B) Confiabilidade
- C) Eficiência de Desempenho
- D) Sustentabilidade

<details>
<summary>Ver resposta</summary>

**Resposta: D**

O pilar de Sustentabilidade foca em minimizar o impacto ambiental, incluindo o uso de energia e recursos.

- A) Excelência Operacional trata de operar, monitorar e melhorar processos.
- B) Confiabilidade trata de recuperação de falhas e atendimento à demanda.
- C) Eficiência de Desempenho trata de usar bem os recursos para atender requisitos de performance.
</details>

### Questão 4 (escolha DUAS)

Quais **duas** opções são vantagens da computação em nuvem?

- A) Trocar despesas de capital por despesas variáveis
- B) Deixar de adivinhar a capacidade necessária
- C) Ter controle total sobre o hardware dos data centers
- D) Garantir um custo mensal idêntico, independente do uso
- E) Eliminar a necessidade de gerenciar a segurança

<details>
<summary>Ver resposta</summary>

**Resposta: A e B**

Na nuvem você paga pelo que consome (despesa variável) e ajusta a capacidade conforme a necessidade real, sem superdimensionar ou ficar sem recursos.

- C) O hardware fica sob responsabilidade da AWS, o cliente não tem controle físico.
- D) O custo varia conforme o uso.
- E) A segurança continua sendo compartilhada, e o cliente segue responsável pela parte dele.
</details>

### Questão 5

No **AWS Cloud Adoption Framework (AWS CAF)**, qual perspectiva trata de treinamento da equipe, cultura e gestão da mudança?

- A) Plataforma
- B) Pessoas
- C) Governança
- D) Operações

<details>
<summary>Ver resposta</summary>

**Resposta: B**

A perspectiva Pessoas (People) cuida de cultura, habilidades, organização e mudança. As seis perspectivas do CAF são Negócios, Pessoas, Governança, Plataforma, Segurança e Operações.

- A) Plataforma trata de arquitetura e infraestrutura técnica.
- C) Governança trata de gestão de portfólio, riscos e conformidade.
- D) Operações trata de monitorar e manter os serviços em produção.
</details>

### Questão 6

Para que servem as **Edge Locations** da AWS?

- A) Entregar conteúdo com baixa latência, aproximando o cache dos usuários finais
- B) Executar instâncias EC2 em qualquer cidade do mundo
- C) Armazenar backups automáticos de bancos de dados RDS
- D) Hospedar as contas de faturamento da organização

<details>
<summary>Ver resposta</summary>

**Resposta: A**

As Edge Locations são usadas por serviços como o Amazon CloudFront para entregar conteúdo mais perto de quem o acessa.

- B) EC2 roda dentro de Regiões e AZs, não em Edge Locations.
- C) Backups do RDS ficam no armazenamento da Região.
- D) Faturamento é um recurso da conta, sem relação com infraestrutura de borda.
</details>

### Questão 7

Uma empresa mantém um banco de dados legado no próprio data center e a aplicação web na AWS, conectados por uma VPN. Que modelo de implantação é esse?

- A) Nuvem pública
- B) Nuvem privada
- C) Híbrida
- D) Serverless

<details>
<summary>Ver resposta</summary>

**Resposta: C**

Misturar recursos on-premises com recursos na nuvem, conectados entre si, caracteriza a implantação híbrida.

- A) Nuvem pública seria ter tudo na AWS.
- B) Nuvem privada seria ter tudo na infraestrutura própria.
- D) Serverless é um modelo de execução, não de implantação.
</details>

---

## Domínio 2: Segurança e Conformidade

### Questão 8

Qual responsabilidade pertence à **AWS** no Modelo de Responsabilidade Compartilhada?

- A) Aplicar patches no sistema operacional convidado das instâncias EC2
- B) Configurar as regras dos Security Groups
- C) Gerenciar usuários e permissões do IAM
- D) Proteger fisicamente os data centers

<details>
<summary>Ver resposta</summary>

**Resposta: D**

A AWS é responsável pela segurança **da** nuvem: instalações físicas, hardware, rede e a camada de virtualização.

- A, B e C) Sistema operacional convidado, regras de firewall e gestão de identidades são responsabilidades do cliente (segurança **na** nuvem).
</details>

### Questão 9

Uma empresa usa o **Amazon RDS**. Qual tarefa continua sendo responsabilidade do cliente?

- A) Controlar quem pode acessar o banco, com Security Groups e usuários do banco
- B) Aplicar patches no sistema operacional do host
- C) Manter o hardware do servidor
- D) Proteger fisicamente o data center

<details>
<summary>Ver resposta</summary>

**Resposta: A**

No RDS, a AWS gerencia hardware e sistema operacional, mas o cliente continua responsável por controle de acesso, configuração de rede e proteção dos dados.

- B, C e D) São tarefas da AWS em serviços gerenciados.
</details>

### Questão 10

Qual é a prática recomendada para o **usuário root** de uma conta AWS?

- A) Criar chaves de acesso do root e usá-las em scripts
- B) Compartilhar a senha do root com a equipe de TI
- C) Ativar MFA e usar o root apenas em tarefas que exigem esse nível de acesso
- D) Usar o root no dia a dia para evitar erros de permissão

<details>
<summary>Ver resposta</summary>

**Resposta: C**

O root tem acesso irrestrito. Proteja com MFA e use usuários ou roles do IAM para o trabalho cotidiano.

- A) Chaves de acesso do root são um risco e devem ser evitadas.
- B) Credenciais do root nunca devem ser compartilhadas.
- D) Isso viola o princípio do menor privilégio.
</details>

### Questão 11

Uma aplicação em uma instância EC2 precisa ler arquivos de um bucket S3, sem armazenar chaves de acesso no código. Qual é a melhor solução?

- A) Gravar chaves de acesso em um arquivo de configuração na instância
- B) Associar um IAM role à instância EC2
- C) Usar as credenciais do usuário root
- D) Compartilhar um único usuário IAM entre todas as aplicações

<details>
<summary>Ver resposta</summary>

**Resposta: B**

Um IAM role entrega credenciais temporárias à instância, sem chaves fixas e com permissões restritas ao necessário.

- A) Chaves em arquivo podem vazar e não rotacionam sozinhas.
- C) Root nunca deve ser usado por aplicações.
- D) Usuário compartilhado dificulta auditoria e amplia o risco.
</details>

### Questão 12

Qual serviço analisa fontes como logs do CloudTrail, VPC Flow Logs e consultas DNS para **detectar atividades suspeitas** na conta?

- A) Amazon Inspector
- B) Amazon Macie
- C) AWS Artifact
- D) Amazon GuardDuty

<details>
<summary>Ver resposta</summary>

**Resposta: D**

O GuardDuty é o serviço de detecção de ameaças que monitora continuamente a conta e as cargas de trabalho.

- A) O Inspector procura vulnerabilidades de software em recursos como EC2, contêineres e Lambda.
- B) O Macie descobre e protege dados sensíveis no S3.
- C) O Artifact fornece relatórios de conformidade.
</details>

### Questão 13

Um auditor solicitou o **relatório SOC** da AWS. Onde a empresa pode baixá-lo?

- A) AWS Artifact
- B) AWS Config
- C) AWS Shield
- D) AWS Trusted Advisor

<details>
<summary>Ver resposta</summary>

**Resposta: A**

O AWS Artifact é o portal de relatórios de auditoria e acordos de conformidade da AWS (como SOC e ISO).

- B) O Config registra e avalia configurações dos seus recursos.
- C) O Shield protege contra DDoS.
- D) O Trusted Advisor dá recomendações de boas práticas.
</details>

### Questão 14

Uma aplicação web precisa **bloquear requisições com padrões de SQL injection**. Qual serviço atende a essa necessidade?

- A) AWS Shield Standard
- B) Amazon GuardDuty
- C) AWS WAF
- D) AWS KMS

<details>
<summary>Ver resposta</summary>

**Resposta: C**

O AWS WAF é um firewall de aplicações web, com regras para filtrar tráfego malicioso como SQL injection e XSS.

- A) O Shield protege contra ataques DDoS.
- B) O GuardDuty detecta ameaças, mas não bloqueia requisições HTTP.
- D) O KMS gerencia chaves de criptografia.
</details>

### Questão 15

Qual serviço permite **criar e controlar as chaves de criptografia** usadas para proteger dados?

- A) AWS Shield
- B) AWS KMS
- C) AWS Artifact
- D) Amazon Inspector

<details>
<summary>Ver resposta</summary>

**Resposta: B**

O AWS Key Management Service (KMS) cria, armazena e controla chaves de criptografia, integrando-se a vários serviços AWS.

- A) Shield é proteção contra DDoS.
- C) Artifact entrega relatórios de conformidade.
- D) Inspector avalia vulnerabilidades.
</details>

### Questão 16

A equipe de segurança precisa descobrir **qual usuário excluiu um bucket S3 e quando**. Qual serviço registra essas chamadas de API?

- A) Amazon CloudWatch
- B) AWS Config
- C) AWS Trusted Advisor
- D) AWS CloudTrail

<details>
<summary>Ver resposta</summary>

**Resposta: D**

O CloudTrail registra as chamadas de API e ações na conta: quem fez, quando e de onde.

- A) O CloudWatch coleta métricas, logs e alarmes de desempenho.
- B) O Config acompanha o histórico de configuração dos recursos, mas não é o registro de quem executou a ação.
- C) O Trusted Advisor dá recomendações, não auditoria de ações.
</details>

---

## Domínio 3: Tecnologia e Serviços da Nuvem

### Questão 17

Qual serviço executa código em resposta a eventos, **sem gerenciar servidores**, com cobrança baseada no tempo de execução?

- A) AWS Lambda
- B) Amazon EC2
- C) Amazon EBS
- D) Amazon RDS

<details>
<summary>Ver resposta</summary>

**Resposta: A**

O Lambda é computação serverless: você envia o código e a AWS provisiona e escala a infraestrutura.

- B) No EC2 você gerencia as instâncias.
- C) O EBS é armazenamento em bloco.
- D) O RDS é banco de dados relacional gerenciado.
</details>

### Questão 18

Uma empresa quer executar contêineres **sem gerenciar servidores ou clusters de instâncias EC2**. Qual opção atende a esse requisito?

- A) Amazon EC2 Auto Scaling
- B) AWS Fargate
- C) Elastic Load Balancing
- D) AWS CloudFormation

<details>
<summary>Ver resposta</summary>

**Resposta: B**

O Fargate é o mecanismo de computação serverless para contêineres, usado com o Amazon ECS e o Amazon EKS.

- A) O Auto Scaling ajusta a quantidade de instâncias EC2, que continuam sob gerenciamento do cliente.
- C) O ELB distribui tráfego entre destinos.
- D) O CloudFormation provisiona infraestrutura como código.
</details>

### Questão 19

Uma empresa precisa guardar dados de conformidade que serão acessados uma ou duas vezes por ano. Esperar até 12 horas pela recuperação é aceitável, e o **menor custo possível** é prioridade. Qual classe do S3 escolher?

- A) S3 Standard
- B) S3 Standard-IA
- C) S3 One Zone-IA
- D) S3 Glacier Deep Archive

<details>
<summary>Ver resposta</summary>

**Resposta: D**

O Glacier Deep Archive é a classe de menor custo, pensada para retenção de longo prazo com acesso raro.

- A) O Standard é para acesso frequente e custa mais.
- B e C) As classes IA têm acesso imediato e são para dados acessados com pouca frequência, mas ainda custam mais que o Deep Archive.
</details>

### Questão 20

Qual serviço oferece um **sistema de arquivos compartilhado e elástico**, acessível ao mesmo tempo por várias instâncias EC2 Linux?

- A) Amazon EBS
- B) Amazon S3
- C) Amazon EFS
- D) Instance Store

<details>
<summary>Ver resposta</summary>

**Resposta: C**

O Amazon EFS é um sistema de arquivos NFS gerenciado que cresce e diminui automaticamente e pode ser montado por várias instâncias.

- A) O EBS é um disco de bloco, em geral anexado a uma instância por vez.
- B) O S3 é armazenamento de objetos, não um sistema de arquivos montável nesse formato.
- D) O Instance Store é temporário e ligado ao host físico.
</details>

### Questão 21

Instâncias em uma **sub-rede privada** precisam baixar atualizações da internet, sem aceitar conexões iniciadas de fora. Qual componente resolve isso?

- A) NAT Gateway
- B) Internet Gateway
- C) VPC Peering
- D) AWS Direct Connect

<details>
<summary>Ver resposta</summary>

**Resposta: A**

O NAT Gateway fica em uma sub-rede pública e permite tráfego de saída das sub-redes privadas, bloqueando conexões iniciadas de fora.

- B) O Internet Gateway dá acesso direto à internet para recursos com IP público, o que não é o caso aqui.
- C) O VPC Peering conecta duas VPCs.
- D) O Direct Connect é um link dedicado com o ambiente on-premises.
</details>

### Questão 22

Qual serviço é um **DNS gerenciado e de alta disponibilidade**, capaz de traduzir nomes de domínio em endereços IP e rotear por saúde ou latência?

- A) Amazon CloudFront
- B) AWS Direct Connect
- C) Amazon Route 53
- D) Amazon API Gateway

<details>
<summary>Ver resposta</summary>

**Resposta: C**

O Route 53 oferece registro de domínios, DNS e políticas de roteamento com verificação de integridade.

- A) O CloudFront é uma CDN.
- B) O Direct Connect é conectividade dedicada.
- D) O API Gateway cria e publica APIs.
</details>

### Questão 23

Uma aplicação precisa de um banco **NoSQL chave-valor**, com latência de milissegundos, escala automática e sem servidores para gerenciar. Qual serviço escolher?

- A) Amazon RDS
- B) Amazon DynamoDB
- C) Amazon Redshift
- D) Amazon Aurora

<details>
<summary>Ver resposta</summary>

**Resposta: B**

O DynamoDB é um banco NoSQL totalmente gerenciado, com escala automática e baixa latência.

- A e D) RDS e Aurora são bancos relacionais.
- C) O Redshift é um data warehouse para análises.
</details>

### Questão 24

Qual é o principal objetivo de habilitar **Multi-AZ** em uma instância do Amazon RDS?

- A) Melhorar a velocidade de leitura distribuindo consultas
- B) Reduzir o custo da instância
- C) Armazenar backups em outra Região
- D) Obter alta disponibilidade, com failover automático para uma réplica standby em outra AZ

<details>
<summary>Ver resposta</summary>

**Resposta: D**

No Multi-AZ, a AWS mantém uma réplica standby em outra AZ e faz o failover automático em caso de falha.

- A) Isso descreve as Read Replicas.
- B) Multi-AZ aumenta o custo, não reduz.
- C) Backup entre Regiões é outro recurso.
</details>

### Questão 25 (escolha DUAS)

Quais **duas** opções são serviços da AWS para executar e orquestrar contêineres?

- A) Amazon S3
- B) Amazon ECS
- C) AWS KMS
- D) Amazon Route 53
- E) Amazon EKS

<details>
<summary>Ver resposta</summary>

**Resposta: B e E**

O Amazon ECS é o orquestrador de contêineres da AWS, e o Amazon EKS é o Kubernetes gerenciado.

- A) S3 é armazenamento de objetos.
- C) KMS gerencia chaves.
- D) Route 53 é DNS.
</details>

### Questão 26

Qual serviço permite **monitorar a utilização de CPU** de instâncias EC2 e disparar alarmes quando um limite é ultrapassado?

- A) Amazon CloudWatch
- B) AWS CloudTrail
- C) AWS Artifact
- D) AWS Organizations

<details>
<summary>Ver resposta</summary>

**Resposta: A**

O CloudWatch coleta métricas, logs e eventos, e permite criar alarmes e ações automáticas.

- B) O CloudTrail registra chamadas de API.
- C) O Artifact fornece relatórios de conformidade.
- D) O Organizations gerencia várias contas.
</details>

---

## Domínio 4: Cobrança, Preços e Suporte

### Questão 27

Uma empresa executa **processamento em lote tolerante a interrupções** e quer o menor custo possível. Qual modelo de compra de EC2 é o mais indicado?

- A) On-Demand
- B) Reserved Instances
- C) Spot Instances
- D) Dedicated Hosts

<details>
<summary>Ver resposta</summary>

**Resposta: C**

As Spot Instances usam capacidade ociosa com grandes descontos, mas podem ser interrompidas pela AWS, o que combina com cargas tolerantes a falhas.

- A) On-Demand é flexível, porém mais caro.
- B) Reserved é indicado para uso estável e contínuo, com compromisso.
- D) Dedicated Hosts atendem a requisitos de licenciamento ou conformidade, não de menor custo.
</details>

### Questão 28

Uma carga de trabalho roda **24 horas por dia, de forma constante**, e continuará assim por pelo menos um ano. Qual opção reduz o custo em troca de um compromisso de uso?

- A) Instâncias Spot
- B) Savings Plans
- C) On-Demand sem compromisso
- D) Uso apenas da camada gratuita

<details>
<summary>Ver resposta</summary>

**Resposta: B**

Os Savings Plans dão desconto em troca do compromisso de gasto por 1 ou 3 anos, ideal para uso previsível e contínuo.

- A) Spot pode ser interrompida e não combina com carga constante e crítica.
- C) On-Demand tem o preço cheio.
- D) A camada gratuita tem limites e não sustenta uma carga contínua de produção.
</details>

### Questão 29

Antes de implantar uma nova arquitetura, a equipe quer **estimar o custo mensal** dos serviços planejados. Qual ferramenta usar?

- A) AWS Pricing Calculator
- B) AWS Cost Explorer
- C) AWS Budgets
- D) AWS Artifact

<details>
<summary>Ver resposta</summary>

**Resposta: A**

O Pricing Calculator estima custos de arquiteturas que ainda não existem.

- B) O Cost Explorer analisa custos e uso que já aconteceram, com projeções.
- C) O Budgets define limites e alertas sobre gastos.
- D) O Artifact não trata de custos.
</details>

### Questão 30

Um gestor quer **receber um alerta por e-mail** quando o gasto previsto do mês ultrapassar US$ 100. Qual serviço permite configurar isso?

- A) AWS Cost Explorer
- B) AWS Pricing Calculator
- C) AWS CloudTrail
- D) AWS Budgets

<details>
<summary>Ver resposta</summary>

**Resposta: D**

O AWS Budgets permite criar orçamentos de custo e uso e enviar alertas quando o gasto real ou previsto passa de um limite.

- A) O Cost Explorer serve para visualizar e analisar custos, sem esse tipo de alerta de orçamento.
- B) O Pricing Calculator estima custos futuros.
- C) O CloudTrail registra chamadas de API.
</details>

---

## Gabarito resumido

| Q | Resp. | Q | Resp. | Q | Resp. | Q | Resp. | Q | Resp. |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| 1 | B | 7 | C | 13 | A | 19 | D | 25 | B, E |
| 2 | C | 8 | D | 14 | C | 20 | C | 26 | A |
| 3 | D | 9 | A | 15 | B | 21 | A | 27 | C |
| 4 | A, B | 10 | C | 16 | D | 22 | C | 28 | B |
| 5 | B | 11 | B | 17 | A | 23 | B | 29 | A |
| 6 | A | 12 | D | 18 | B | 24 | D | 30 | D |

## Seu resultado

| Acertos | Percentual | O que fazer |
|:-:|:-:|---|
| 27 a 30 | 90% ou mais | Excelente. Parta para o Simulado 02 e revise só os erros. |
| 24 a 26 | 80% a 89% | No caminho certo. Revise os tópicos errados e refaça o simulado depois. |
| 18 a 23 | 60% a 79% | Releia as pastas dos domínios em que errou mais e refaça os labs. |
| Menos de 18 | Abaixo de 60% | Volte ao roteiro de estudos e estude por domínio antes de tentar de novo. |

> A pontuação oficial do exame usa uma escala de 100 a 1000, com mínimo de 700, e não equivale diretamente a uma porcentagem de acertos. Use este percentual apenas como referência de estudo.

### Onde revisar cada domínio

| Errou mais em | Revise |
|---|---|
| Questões 1 a 7 | [`01-conceitos-de-nuvem/`](../01-conceitos-de-nuvem) |
| Questões 8 a 16 | [`02-seguranca-e-conformidade/`](../02-seguranca-e-conformidade) |
| Questões 17 a 26 | [`03-tecnologia-e-servicos/`](../03-tecnologia-e-servicos) |
| Questões 27 a 30 | [`04-cobranca-e-suporte/`](../04-cobranca-e-suporte) |

---

Encontrou um erro ou quer sugerir uma melhoria? Abra uma *issue* ou envie um *Pull Request*. Se este simulado ajudou, deixe uma estrela no repositório.
