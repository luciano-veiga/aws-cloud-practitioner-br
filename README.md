# AWS Cloud Practitioner (CLF-C02): Guia de Estudos em Português

![Exame](https://img.shields.io/badge/AWS-CLF--C02-FF9900?logo=amazonaws&logoColor=white)
![Idioma](https://img.shields.io/badge/idioma-pt--BR-009C3B)
![Licença](https://img.shields.io/badge/licen%C3%A7a-MIT-blue)
![Status](https://img.shields.io/badge/status-em%20constru%C3%A7%C3%A3o-yellow)
![Contribuições](https://img.shields.io/badge/PRs-bem--vindos-brightgreen)

> Material independente, **não afiliado à AWS**. Marcas pertencem aos seus donos. Sempre confira o [guia oficial do exame](https://aws.amazon.com/certification/certified-cloud-practitioner/), pois a AWS pode atualizar o conteúdo.

---

## Bem-vindo(a)

Este repositório foi preparado para guiar você rumo à aprovação na certificação **AWS Certified Cloud Practitioner (CLF-C02)**.

Aqui você encontra teoria objetiva organizada pelos 4 domínios oficiais, laboratórios práticos passo a passo, fundamentos técnicos de apoio e simulados com explicação de cada alternativa. Não precisa ter experiência prévia com nuvem. Siga o roteiro no seu ritmo e pratique bastante.

**Sobre o autor:** Luciano Veiga, mais de 20 anos em TI (NOC, suporte técnico, CCTV e instrução), certificado AWS Cloud Practitioner e AWS Solutions Architect Associate.
[LinkedIn](https://www.linkedin.com/in/lucianoveiga-ti/) | [GitHub](https://github.com/luciano-veiga) | [Site](https://lucianoveiga.is-a.dev/)

---

## Sumário

1. [Sobre o exame](#sobre-o-exame)
2. [Como usar este repositório](#como-usar-este-repositório)
3. [Os 4 domínios](#os-4-domínios-do-exame)
4. [Fundamentos técnicos](#fundamentos-técnicos)
5. [Laboratórios práticos](#laboratórios-práticos-hands-on)
6. [Simulados e checagem de conhecimento](#simulados-e-checagem-de-conhecimento)
7. [Recursos oficiais](#recursos-oficiais)
8. [Estrutura de pastas](#estrutura-de-pastas)
9. [Plano de estudos](#plano-de-estudos-sugerido)
10. [Como contribuir](#como-contribuir)
11. [Licença e aviso legal](#licença-e-aviso-legal)

---

## Sobre o exame

| Item | Detalhe |
|---|---|
| Certificação | AWS Certified Cloud Practitioner |
| Código | CLF-C02 |
| Nível | Foundational (fundamentos) |
| Questões | 65 (50 pontuadas e 15 não pontuadas, sem identificação) |
| Formato | Múltipla escolha e múltipla resposta |
| Duração | 90 minutos |
| Nota para aprovação | **700 de 1000** (escala de 100 a 1000) |
| Modalidade | Centro Pearson VUE ou online com fiscalização |
| Validade | 3 anos |

> Confirme valores, idiomas e regras atuais na [página oficial da certificação](https://aws.amazon.com/certification/certified-cloud-practitioner/).

### Peso dos domínios

| Domínio | Tema | Peso |
|:---:|---|:---:|
| 1 | Conceitos de Nuvem | 24% |
| 2 | Segurança e Conformidade | 30% |
| 3 | Tecnologia e Serviços da Nuvem | 34% |
| 4 | Cobrança, Preços e Suporte | 12% |

---

## Como usar este repositório

1. Faça um **fork** ou **star** para acompanhar as atualizações.
2. Siga a ordem das pastas `01` a `04`. Cada uma termina com um *Knowledge Check*.
3. Faça os laboratórios em `labs-praticos/` na sua conta AWS (use o Free Tier e **sempre limpe os recursos no final**).
4. Teste-se em `simulados-e-exercicios/` e anote o que errou.
5. Antes do exame, refaça os simulados e leia os cheatsheets.

> **Alerta de custos:** crie um alerta no AWS Budgets antes de qualquer laboratório. Confira as regras atuais do [AWS Free Tier](https://aws.amazon.com/free/).

---

## Os 4 domínios do exame

### Domínio 1: Conceitos de Nuvem (24%)

Pasta: [`01-conceitos-de-nuvem/`](./01-conceitos-de-nuvem)

- [ ] Proposta de valor da AWS: agilidade, elasticidade, economia de escala, troca de CapEx por OpEx
- [ ] Modelos de implantação: nuvem pública, privada, híbrida
- [ ] Infraestrutura global: Regiões, Zonas de Disponibilidade, Edge Locations
- [ ] **AWS Well-Architected Framework** e seus 6 pilares:

| Pilar | Foco |
|---|---|
| Excelência Operacional | Operar, monitorar e melhorar processos |
| Segurança | Proteger dados, sistemas e ativos |
| Confiabilidade | Recuperar-se de falhas e atender à demanda |
| Eficiência de Desempenho | Usar recursos de forma eficiente |
| Otimização de Custos | Evitar gastos desnecessários |
| Sustentabilidade | Reduzir o impacto ambiental |

- [ ] **AWS Cloud Adoption Framework (AWS CAF)**: perspectivas de negócios, pessoas, governança, plataforma, segurança e operações
- [ ] Estratégias de migração (os 7 Rs) e noções do AWS Migration Hub

### Domínio 2: Segurança e Conformidade (30%)

Pasta: [`02-seguranca-e-conformidade/`](./02-seguranca-e-conformidade)

- [ ] **Modelo de Responsabilidade Compartilhada**: AWS cuida *da* nuvem, você cuida *na* nuvem
- [ ] **AWS IAM**: usuários, grupos, roles, políticas, MFA, princípio do menor privilégio, usuário root
- [ ] Criptografia em repouso e em trânsito, **AWS KMS**
- [ ] **AWS Artifact**: relatórios de conformidade e acordos
- [ ] **Amazon GuardDuty**: detecção de ameaças
- [ ] **AWS Shield**: proteção contra DDoS
- [ ] **AWS WAF**: firewall de aplicações web
- [ ] Complementos: Security Groups e NACLs, Amazon Inspector, AWS Security Hub, AWS CloudTrail, AWS Config, AWS Organizations

### Domínio 3: Tecnologia e Serviços da Nuvem (34%)

Pasta: [`03-tecnologia-e-servicos/`](./03-tecnologia-e-servicos)

| Categoria | Serviços para estudar |
|---|---|
| Computação | EC2, Lambda, ECS, Fargate, Elastic Beanstalk, Auto Scaling, ELB |
| Armazenamento | S3 (classes de armazenamento), S3 Glacier, EBS, EFS, Storage Gateway |
| Redes | VPC, sub-redes, Internet Gateway, NAT Gateway, Route 53, CloudFront, Direct Connect, VPN |
| Bancos de dados | RDS, Aurora, DynamoDB, ElastiCache, Redshift |
| Integração e monitoramento | SQS, SNS, CloudWatch, CloudFormation |
| IA/ML (visão geral) | SageMaker, Rekognition, Comprehend, Amazon Q, Bedrock |

### Domínio 4: Cobrança, Preços e Suporte (12%)

Pasta: [`04-cobranca-e-suporte/`](./04-cobranca-e-suporte)

- [ ] Modelos de compra: **On-Demand, Reserved Instances, Spot, Savings Plans, Dedicated Hosts**
- [ ] **AWS Pricing Calculator**: estimar custos antes de implantar
- [ ] **AWS Cost Explorer**: analisar custos passados e projeções
- [ ] **AWS Budgets**: alertas de orçamento e uso
- [ ] Billing consolidado com AWS Organizations, tags de alocação de custos
- [ ] **Planos de AWS Support**: comparar os níveis disponíveis, tempos de resposta e acesso ao TAM (confira a [página atual de planos](https://aws.amazon.com/premiumsupport/plans/))
- [ ] Ferramentas de apoio: AWS Trusted Advisor, AWS Health Dashboard, AWS Marketplace

---

## Fundamentos técnicos

Base prática que facilita o entendimento dos serviços. Material em `labs-praticos/fundamentos/`.

### 1. Linux essencial

| Comando | Uso |
|---|---|
| `ls`, `cd`, `pwd` | Navegar entre diretórios |
| `cat`, `less`, `tail -f` | Ler arquivos e acompanhar logs |
| `chmod`, `chown` | Permissões (essencial para chaves `.pem`) |
| `ssh -i chave.pem ec2-user@IP` | Acessar uma instância EC2 |
| `sudo`, `dnf`/`yum`/`apt` | Administrar e instalar pacotes |
| `systemctl status servico` | Gerenciar serviços |
| `curl`, `ping`, `ss -tulpn` | Testar conectividade e portas |

### 2. Automação com Python e Boto3

```python
import boto3

s3 = boto3.client("s3")

# Lista os buckets da conta
for bucket in s3.list_buckets()["Buckets"]:
    print(bucket["Name"])
```

Antes de rodar: instale o AWS CLI, execute `aws configure` com um usuário IAM de **menor privilégio** e nunca versione credenciais.

### 3. Redes básicas

CIDR e máscara de sub-rede, IP público x privado, portas comuns (22, 80, 443, 3306), DNS, NAT, diferença entre Security Group (stateful) e NACL (stateless).

### 4. Banco de dados: MySQL no RDS

Conceitos de banco relacional, criação de uma instância RDS MySQL, Multi-AZ x Read Replica, backups automáticos, conexão com `mysql -h ENDPOINT -u admin -p`.

---

## Laboratórios práticos (Hands-on)

Cada lab fica em `labs-praticos/NN-nome-do-lab/` com objetivo, pré-requisitos, passo a passo, custo estimado e **seção de limpeza**.

| Lab | Tema | Domínio | Nível |
|:---:|---|:---:|:---:|
| 01 | Criar conta, ativar MFA e configurar alerta no Budgets | 2 e 4 | Iniciante |
| 02 | Criar usuário, grupo e política no IAM | 2 | Iniciante |
| 03 | Lançar uma instância EC2 e acessar via SSH | 3 | Iniciante |
| 04 | Hospedar um site estático no S3 | 3 | Iniciante |
| 05 | Criar uma VPC com sub-redes pública e privada | 3 | Intermediário |
| 06 | Criar um banco MySQL no RDS e conectar a partir da EC2 | 3 | Intermediário |
| 07 | Função Lambda acionada por evento do S3 | 3 | Intermediário |
| 08 | Explorar custos com Cost Explorer e Pricing Calculator | 4 | Iniciante |
| 09 | Script Python (Boto3) para listar recursos da conta | 3 | Intermediário |

**Modelo de cada lab:** Objetivo > Pré-requisitos > Arquitetura > Passo a passo > Validação > Custo estimado > Limpeza > Desafio extra.

---

## Simulados e checagem de conhecimento

### Knowledge Checks por módulo

Cada pasta de domínio termina com um arquivo `knowledge-check.md` contendo questões rápidas com gabarito comentado, explicando por que a alternativa correta está certa **e por que as outras estão erradas**.

### Simulados do repositório

Pasta: [`simulados-e-exercicios/`](./simulados-e-exercicios)

| Simulado | Questões | Foco | Status |
|---|:---:|---|---|
| [Simulado 01 interativo](https://luciano-veiga.github.io/aws-cloud-practitioner-br/simulados-e-exercicios/simulado-01.html) ([versão em texto](./simulados-e-exercicios/simulado-01.md)) | 30 | Visão geral dos 4 domínios | Disponível |
| Simulado 02 | 30 | Segurança e Conformidade | Em breve |
| Simulado 03 | 30 | Tecnologia e Serviços | Em breve |
| Simulado 04 | 30 | Cobrança e Suporte | Em breve |

### Plataformas para praticar

- [AWS Skill Builder](https://skillbuilder.aws/): conjunto oficial de questões de prática e curso de preparação para o exame (verifique o que está gratuito no momento)
- Simulados deste repositório (originais, em português)

> **Aviso importante:** não utilize nem compartilhe *braindumps* ou questões reais vazadas. Isso viola o acordo de certificação da AWS e não prepara você de verdade. Todas as questões deste repositório são originais.

---

## Recursos oficiais

| Recurso | Link |
|---|---|
| Página da certificação e guia do exame | [aws.amazon.com/certification](https://aws.amazon.com/certification/certified-cloud-practitioner/) |
| Documentação oficial da AWS | [docs.aws.amazon.com](https://docs.aws.amazon.com/) |
| Curso gratuito *AWS Cloud Practitioner Essentials* | [skillbuilder.aws](https://skillbuilder.aws/) |
| AWS Skill Builder | [skillbuilder.aws](https://skillbuilder.aws/) |
| AWS Educate | [aws.amazon.com/education/awseducate](https://aws.amazon.com/education/awseducate/) |
| AWS re:Post (comunidade) | [repost.aws](https://repost.aws/) |
| Well-Architected Framework | [aws.amazon.com/architecture/well-architected](https://aws.amazon.com/architecture/well-architected/) |
| Cloud Adoption Framework | [aws.amazon.com/cloud-adoption-framework](https://aws.amazon.com/cloud-adoption-framework/) |
| Pricing Calculator | [calculator.aws](https://calculator.aws/) |
| Free Tier | [aws.amazon.com/free](https://aws.amazon.com/free/) |
| Whitepaper de Responsabilidade Compartilhada | [aws.amazon.com/compliance/shared-responsibility-model](https://aws.amazon.com/compliance/shared-responsibility-model/) |

---

## Estrutura de pastas

```
aws-cloud-practitioner-br/
├── README.md
├── 01-conceitos-de-nuvem/
├── 02-seguranca-e-conformidade/
├── 03-tecnologia-e-servicos/
├── 04-cobranca-e-suporte/
├── labs-praticos/
│   ├── fundamentos/
│   └── NN-nome-do-lab/
├── simulados-e-exercicios/
├── cheatsheets/
├── CONTRIBUTING.md
├── LICENSE
└── .github/
    ├── ISSUE_TEMPLATE/
    └── workflows/
```

Dentro de cada pasta de domínio:

```
0X-nome-do-dominio/
├── README.md              (visão geral e objetivos)
├── NN-topico.md           (um arquivo por tópico)
└── knowledge-check.md     (questões com gabarito comentado)
```

---

## Plano de estudos sugerido

| Semana | Foco | Entrega |
|:---:|---|---|
| 1 | Domínio 1 + Labs 01 e 02 | Knowledge Check 1 |
| 2 | Domínio 2 + Fundamentos de Linux | Knowledge Check 2 |
| 3 | Domínio 3 (computação e armazenamento) + Labs 03 e 04 | Knowledge Check 3a |
| 4 | Domínio 3 (redes e bancos) + Labs 05, 06 e 07 | Knowledge Check 3b |
| 5 | Domínio 4 + Lab 08 | Knowledge Check 4 |
| 6 | Revisão geral e simulados | Meta: acima de 80% nos simulados |

Ritmo mais curto? Condense em 2 semanas priorizando os domínios 2 e 3, que somam 64% da prova.

---

## Como contribuir

Contribuições são muito bem-vindas.

1. Abra uma *issue* descrevendo a correção ou sugestão.
2. Faça um fork, crie uma branch (`feat/nome-da-mudanca`) e abra um *Pull Request*.
3. Use mensagens de commit no padrão [Conventional Commits](https://www.conventionalcommits.org/pt-br/).
4. Cite a fonte oficial para qualquer afirmação técnica.

Procure as issues com os rótulos `good first issue` e `help wanted`. Veja mais em [CONTRIBUTING.md](./CONTRIBUTING.md).

### Contribuidores

Obrigado a todos que ajudam a melhorar este material.

---

## Licença e aviso legal

- Conteúdo e código sob licença [MIT](./LICENSE).
- Este projeto é independente e não possui vínculo com a Amazon Web Services, Inc.
- Nenhum conteúdo aqui é proveniente de questões reais do exame.
- Nunca publique credenciais, IDs de conta ou dados sensíveis em issues, PRs ou prints.

---

Se este material ajudou você, deixe uma estrela no repositório e compartilhe com quem está começando na nuvem. Boa prova!
