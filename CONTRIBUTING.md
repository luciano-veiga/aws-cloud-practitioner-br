# Como contribuir

Obrigado por querer ajudar! Este repositório existe para apoiar quem estuda para a certificação **AWS Certified Cloud Practitioner (CLF-C02)**, e toda contribuição que melhore o material é bem-vinda: correções, novas questões, labs, traduções e sugestões.

## Formas de contribuir

| Tipo | Como |
|---|---|
| Erro técnico ou de digitação | Abra uma *issue* com o arquivo, a linha e a fonte oficial que comprova o ajuste |
| Dúvida ou sugestão | Abra uma *issue* descrevendo a ideia |
| Nova questão de simulado | Envie um *Pull Request* seguindo o [modelo de questão](#modelo-de-questão) |
| Novo lab ou tópico | Abra uma *issue* antes, para alinharmos o escopo, e depois envie o PR |
| Atualização por mudança no exame | Cite a fonte oficial (guia do exame ou documentação da AWS) |

Procure as issues com os rótulos `good first issue` e `help wanted` se for sua primeira contribuição.

## Regras importantes

1. **Nada de questões reais de prova nem *braindumps*.** Isso viola o acordo de certificação da AWS. Todas as questões devem ser originais, escritas por você com base no guia oficial e na documentação.
2. **Cite a fonte** de qualquer afirmação técnica, preferindo a documentação oficial da AWS.
3. **Nunca inclua dados sensíveis**: chaves de acesso, IDs de conta, e-mails, tokens ou dados de empresas, nem em texto, nem em prints.
4. **Direitos autorais**: não copie trechos de cursos, livros ou sites de terceiros. Escreva com suas palavras.
5. **Respeito**: trate todos com cordialidade. Críticas são sobre o conteúdo, nunca sobre as pessoas.

## Passo a passo para enviar um Pull Request

```bash
# 1. Faça um fork pelo GitHub e clone o seu fork
git clone https://github.com/SEU_USUARIO/aws-cloud-practitioner-br.git
cd aws-cloud-practitioner-br

# 2. Crie uma branch para a sua mudança
git checkout -b feat/nome-da-mudanca

# 3. Faça as alterações, depois commit e push
git add .
git commit -m "feat(simulados): add questao sobre IAM roles"
git push origin feat/nome-da-mudanca
```

4. No GitHub, abra o *Pull Request* para a branch `main` descrevendo o que mudou e por quê.
5. Responda aos comentários da revisão. Pequenos ajustes são normais.

## Padrão de commits

Usamos [Conventional Commits](https://www.conventionalcommits.org/pt-br/):

| Prefixo | Uso |
|---|---|
| `feat` | Novo conteúdo (tópico, lab, questão, simulado) |
| `fix` | Correção de erro técnico ou de digitação |
| `docs` | Ajustes em README, CONTRIBUTING e textos gerais |
| `chore` | Organização, automações e manutenção |

Exemplos: `feat(labs): add lab 03 de EC2`, `fix(simulado-01): corrige gabarito da questao 12`.

## Modelo de questão

Toda questão deve ter enunciado, alternativas, resposta e explicação do **motivo de cada alternativa errada**.

```markdown
### Questão X

Enunciado com um cenário curto e objetivo.

- A) Alternativa
- B) Alternativa
- C) Alternativa
- D) Alternativa

<details>
<summary>Ver resposta</summary>

**Resposta: C**

Por que a C está correta.

- A) Por que está errada.
- B) Por que está errada.
- D) Por que está errada.
</details>
```

Orientações:

- Indique o domínio do exame ao qual a questão pertence.
- Use cenários realistas e evite pegadinhas de interpretação de texto.
- Para questões de múltipla resposta, escreva "(escolha DUAS)" no enunciado.
- Distribua as respostas corretas entre as letras A, B, C e D.

## Modelo de lab

Cada lab fica em `labs-praticos/NN-nome-do-lab/README.md` com as seções:

1. Objetivo
2. Pré-requisitos
3. Arquitetura (diagrama ou descrição)
4. Passo a passo
5. Validação
6. Custo estimado e uso do Free Tier
7. **Limpeza** dos recursos criados (obrigatória)
8. Desafio extra (opcional)

## Dúvidas

Abra uma *issue* com o rótulo `question`. Quando possível, responderemos por lá, para que a resposta ajude outras pessoas também.

Ao contribuir, você concorda que o seu trabalho será publicado sob a licença do repositório (veja o arquivo [LICENSE](./LICENSE)).

Muito obrigado por ajudar a tornar este material melhor!
