---
materia: Engenharia de Software I
tipo: aula
status: refeito_por_ia
fonte:
  - 08-parte1-Gerência de Requisitos + Gestão de Mudanças.pdf
  - 07-parte1-Requisitos + Gerência de Requisitos.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - gerencia-de-requisitos
  - mudancas
  - configuracao
---

# Gerência de Requisitos, Controle de Mudanças e Configuração

Esta nota explica como controlar requisitos e mudanças durante o desenvolvimento. O ponto central é que requisitos mudam; o problema não é a mudança existir, mas acontecer sem análise, rastreabilidade e controle.

## Palavras-chave

- Gerência de requisitos
- Controle de mudanças
- Baseline
- [[07 - Docker Parte 1 - Containers, Imagens, Arquitetura e Dockerfile|Gerência de configuração]]
- Impacto
- Dependência
- Rastreabilidade
- Versão
- Itens de configuração

## Resumo geral da aula

Gerência de requisitos é a atividade de identificar, controlar e rastrear requisitos e suas modificações ao longo do projeto. Conforme o desenvolvimento evolui, requisitos podem ser alterados, removidos ou adicionados.

O controle de mudanças estabelece um caminho formal para avaliar solicitações. A gerência de configuração controla os itens do software que compõem uma baseline, reduzindo o impacto de modificações e mantendo histórico do que foi produzido.

---

## 1. Gerência de requisitos

### Para que serve

Serve para manter controle sobre requisitos durante todo o projeto.

### Explicação detalhada e realista

Requisitos não permanecem sempre iguais. Clientes mudam de ideia, regras de negócio evoluem, restrições técnicas aparecem e novas necessidades surgem. Sem gerência, a equipe perde controle do que foi combinado, do que mudou, por que mudou e quais partes do sistema foram afetadas.

Gerenciar requisitos envolve identificar cada requisito de forma única, registrar sua origem, controlar versões, mapear dependências e acompanhar mudanças.

### Metáfora

Gerência de requisitos é como controle de estoque. Se você não sabe o que entrou, saiu, mudou ou está reservado, não consegue administrar o produto.

### Situações de uso / exemplo real

Um requisito RF001 dizia “o sistema deve emitir relatório mensal”. Depois o cliente pede relatório por período, setor e usuário. Essa mudança precisa ser registrada, avaliada e aprovada.

### Como posso aplicar no dia a dia

Numere requisitos e mantenha histórico. Não altere requisitos antigos sem registrar o que mudou.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[10 - Manutenção de Software e Rastreabilidade]]

---

## 2. Controle de mudanças

### Para que serve

Serve para avaliar e conduzir mudanças de forma planejada.

### Explicação detalhada e realista

Controle de mudanças evita que qualquer solicitação seja implementada imediatamente sem análise. Uma mudança pode parecer pequena, mas afetar prazo, custo, arquitetura, testes, documentação, [[09 - Banco de Dados e SGBD - Parte 1|banco de dados]] e outros requisitos.

O processo recomendado envolve checar a validade da solicitação, identificar requisitos afetados, mapear dependências, estimar custos, explicar impacto ao solicitante e obter aceite.

### Metáfora

Controle de mudanças é como autorização para reforma em um prédio. Mudar uma parede pode parecer simples, mas pode afetar estrutura, elétrica, hidráulica e segurança.

### Situações de uso / exemplo real

Cliente pede para permitir cancelar venda após faturamento. Isso pode afetar estoque, financeiro, nota fiscal, comissão, relatórios e auditoria.

### Como posso aplicar no dia a dia

Antes de aceitar mudança, responda: qual requisito muda? Quem pediu? Por quê? O que será afetado? Quanto tempo custa? Quem aprova?

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[10 - Manutenção de Software e Rastreabilidade]]
- [[08 - Modelos de Desenvolvimento]]

---

## 3. Baseline de requisitos

### Para que serve

Serve para criar um ponto de referência aprovado dos requisitos.

### Explicação detalhada e realista

Baseline é uma versão congelada e controlada de um conjunto de itens. No caso de requisitos, ela permite saber o que era o requisito original, o que foi introduzido, o que foi alterado e o que foi descartado.

Sem baseline, a equipe pode discutir eternamente sobre “o combinado”. Com baseline, há uma referência documentada.

### Metáfora

Baseline é como tirar uma foto oficial do estado do projeto naquele momento. Depois, qualquer mudança pode ser comparada com essa foto.

### Situações de uso / exemplo real

Após aprovar RF001 a RF020, a equipe cria uma baseline. Se o cliente pede mudança no RF010, a alteração é registrada em relação à versão aprovada.

### Como posso aplicar no dia a dia

Salve versões dos documentos de requisitos. Use nomes como `requisitos_v1`, `requisitos_v2`, ou controle via Git.

### Relações com outras notas

- [[02 - Ciclo de Vida de Software, Produto, Processo e Projeto]]

---

## 4. Gerência de configuração

### Para que serve

Serve para controlar versões e mudanças em artefatos do software.

### Explicação detalhada e realista

Gerência de configuração envolve critérios, técnicas e ferramentas para controlar modificações aplicadas ao software durante o projeto. Itens de configuração podem incluir código-fonte, documentos de requisitos, modelos, scripts de banco, arquivos de configuração, casos de teste e documentação.

Ao final de fases ou marcos importantes, baselines são criadas. Isso permite recuperar versões, comparar mudanças e reduzir impacto de alterações.

### Metáfora

Gerência de configuração é como controle de versões de um documento importante. Sem isso, surgem arquivos como “final”, “final2”, “final_agora_vai” e ninguém sabe qual é o correto.

### Situações de uso / exemplo real

Uma equipe usa Git para controlar código, versiona scripts SQL, mantém documentos em repositório e aprova mudanças por pull request.

### Como posso aplicar no dia a dia

Use Git. Registre commits claros. Separe versões estáveis. Documente mudanças importantes.

### Relações com outras notas

- [[03 - Processos de Software, Atividades Fundamentais, CMMI e MPS.br]]
- [[10 - Manutenção de Software e Rastreabilidade]]

## Pontos importantes para prova ou revisão

- Requisitos mudam ao longo do projeto.
- Gerência de requisitos identifica, controla e rastreia requisitos.
- Controle de mudanças avalia validade, impacto, dependências e custo.
- Baseline é uma referência aprovada.
- [[07 - Docker Parte 1 - Containers, Imagens, Arquitetura e Dockerfile|Gerência de configuração]] controla itens modificáveis do software.
- Mudanças sem controle aumentam retrabalho e risco.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Gerência de requisitos | Controle de requisitos e suas mudanças |
| Controle de mudanças | Processo para avaliar e aprovar alterações |
| Baseline | Versão aprovada e controlada de um conjunto de itens |
| Item de configuração | Artefato sujeito a controle de versão |
| Impacto | Efeito de uma mudança sobre requisitos, código, custo ou prazo |
| Dependência | Relação entre requisitos ou componentes |

## Possíveis notas futuras

- Git e gerência de configuração
- Change request
- Matriz de impacto
- Baseline em projetos ágeis

## Fonte

Materiais usados como base:

- 08-parte1-Gerência de Requisitos + Gestão de Mudanças.pdf
- 07-parte1-Requisitos + Gerência de Requisitos.pdf
