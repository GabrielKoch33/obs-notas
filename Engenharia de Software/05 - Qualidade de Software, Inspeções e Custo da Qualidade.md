---
materia: Engenharia de Software I
tipo: aula
status: refeito_por_ia
fonte:
  - 04-parte1-Qualidade de Software.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - qualidade
  - inspeção
  - defeitos
---

# Qualidade de Software, Inspeções e Custo da Qualidade

Esta nota trata qualidade de software como um conceito técnico e gerenciável, não apenas como opinião. O foco é entender que qualidade depende de requisitos, processo, inspeções, prevenção de defeitos e controle contínuo.

## Palavras-chave

- Qualidade de software
- Requisitos
- Defeito
- Erro
- Falha
- Inspeção
- Checklist
- Garantia da qualidade
- Custo da qualidade
- Prevenção
- Avaliação

## Resumo geral da aula

Qualidade em software está relacionada ao atendimento dos requisitos explícitos e implícitos do cliente. Na visão profissional, qualidade pode e deve ser definida, medida, monitorada, gerenciada e melhorada.

A qualidade não aparece apenas no final do projeto. Ela é construída ao longo do processo por meio de métodos adequados, verificação, inspeções, testes, controle de mudanças, gestão de requisitos e prevenção de defeitos.

---

## 1. Qualidade como atendimento aos requisitos

### Para que serve

Serve para transformar qualidade em algo controlável, evitando que ela seja tratada apenas como gosto pessoal.

### Explicação detalhada e realista

Na visão popular, qualidade pode ser associada a luxo, sofisticação ou preferência. Na Engenharia de Software, qualidade está ligada à conformidade com requisitos e à capacidade de satisfazer necessidades explícitas e implícitas.

Isso significa que um software bonito, caro ou complexo não é necessariamente de qualidade. Se ele não atende os requisitos, se é inseguro, se falha em operações importantes ou se não resolve o problema do usuário, sua qualidade é baixa.

### Metáfora

Qualidade de software é como uma chave. Ela pode ser bonita, brilhante e cara, mas se não abre a fechadura correta, não cumpre sua função.

### Situações de uso / exemplo real

Um sistema de login com interface moderna, mas que permite acesso indevido, falha em um requisito essencial de segurança. Logo, não tem qualidade adequada.

### Como posso aplicar no dia a dia

Ao avaliar um projeto, pergunte: ele cumpre o que foi pedido? O comportamento está correto? É fácil de usar? É seguro? É testável? É possível modificar depois?

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[06 - Atributos e Características de Qualidade de Software]]

---

## 2. Complexidade e qualidade

### Para que serve

Serve para entender por que qualidade em software é difícil de garantir.

### Explicação detalhada e realista

Software possui muitas interações internas. Pequenas mudanças podem afetar regras, telas, banco de dados, permissões, integrações e relatórios. Diferente de produtos físicos, o software pode crescer em complexidade de forma invisível.

Essa complexidade torna a qualidade dependente de processo. Se a equipe abandona planos, ignora procedimentos, não revisa requisitos e testa pouco, o produto pode funcionar parcialmente, mas com defeitos, prazo maior, custo maior e menos funcionalidade.

### Metáfora

Software complexo é como uma teia. Puxar um fio pode mexer em vários outros pontos. Sem cuidado, uma alteração aparentemente simples causa efeitos colaterais.

### Situações de uso / exemplo real

Alterar uma regra de desconto pode afetar carrinho, relatório financeiro, nota fiscal, comissão de vendedor e integração com pagamento.

### Como posso aplicar no dia a dia

Não trate mudanças como isoladas sem verificar impactos. Sempre procure onde a regra aparece e que testes precisam ser refeitos.

### Relações com outras notas

- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]
- [[10 - Manutenção de Software e Rastreabilidade]]

---

## 3. Inspeções de software

### Para que serve

Servem para encontrar defeitos antes da execução do sistema ou antes que eles cheguem ao usuário.

### Explicação detalhada e realista

Inspeções são revisões sistemáticas de artefatos. Elas podem ser aplicadas a requisitos, projeto, configuração, dados de teste, código e documentação. Sua vantagem é que não exigem necessariamente executar o sistema.

Um checklist de inspeção ajuda a procurar defeitos comuns. Em requisitos, o checklist pode verificar ambiguidade, fonte, testabilidade, rastreabilidade e relação com objetivos do produto. Em código, pode verificar limites de vetor, inicialização de variáveis, repetição de loops e tratamento de exceções.

### Metáfora

Inspeção é como revisar uma planta antes de construir. Corrigir erro no papel é muito mais barato do que quebrar uma parede pronta.

### Situações de uso / exemplo real

Antes de implementar um requisito, a equipe verifica se ele é claro, testável, numerado, rastreável e não viola o escopo. Isso evita implementar algo mal entendido.

### Como posso aplicar no dia a dia

Antes de entregar um trabalho, revise com checklist: requisito claro? Código compila? Casos extremos foram testados? Variáveis têm nomes bons? Há divisão por zero? Há tratamento para entradas inválidas?

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 4. Métodos ágeis e inspeções

### Para que serve

Serve para entender que a revisão pode ocorrer de forma formal ou contínua, dependendo do processo adotado.

### Explicação detalhada e realista

Processos ágeis nem sempre usam inspeções formais pesadas. Em vez disso, podem usar revisão contínua, colaboração, pair programming e práticas como “verifique antes do check-in”. No Extreme Programming, a programação em pares funciona como uma inspeção contínua: duas pessoas acompanham cada linha de código.

Isso não elimina a necessidade de qualidade. Apenas muda a forma de controle. A inspeção formal pode ser substituída por práticas frequentes de revisão, testes automatizados, integração contínua e feedback.

### Metáfora

Inspeção formal é como vistoria agendada. Revisão ágil contínua é como ter sensores monitorando o tempo todo.

### Situações de uso / exemplo real

Em uma equipe ágil, antes de enviar uma alteração ao repositório principal, outro desenvolvedor revisa o código via pull request. Isso reduz erros e compartilha conhecimento.

### Como posso aplicar no dia a dia

Peça para outra pessoa revisar seu código ou explique seu código em voz alta. Muitas falhas aparecem quando você tenta justificar sua própria lógica.

### Relações com outras notas

- [[03 - Processos de Software, Atividades Fundamentais, CMMI e MPS.br]]
- [[04 - Modelos de Desenvolvimento de Software - Cascata, Incremental, Iterativo, V, Espiral e Prototipação]]

---

## 5. Custo da qualidade

### Para que serve

Serve para mostrar que investir em qualidade custa, mas não investir costuma custar mais.

### Explicação detalhada e realista

O custo da qualidade envolve atividades de prevenção, avaliação e falhas. Prevenção inclui treinamento, boas práticas, padrões, revisão e planejamento. Avaliação inclui testes, auditorias e inspeções. Falhas incluem correção de defeitos internos ou problemas encontrados pelo cliente.

Quanto mais tarde um defeito é descoberto, maior tende a ser seu custo. Um erro em requisito corrigido antes da implementação é barato. O mesmo erro descoberto em produção pode envolver retrabalho, suporte, correção emergencial, perda de confiança e impacto financeiro.

### Metáfora

É mais barato colocar freio bom no carro do que pagar acidente, conserto, hospital e processo judicial.

### Situações de uso / exemplo real

Um erro em cálculo financeiro descoberto após meses em produção pode exigir correção de banco, reemissão de relatórios, contato com clientes e auditoria.

### Como posso aplicar no dia a dia

Teste cedo. Revise cedo. Valide requisitos cedo. Quanto antes um erro aparece, menos caro ele é.

### Relações com outras notas

- [[06 - Atributos e Características de Qualidade de Software]]
- [[10 - Manutenção de Software e Rastreabilidade]]

---

## 6. Defeito, erro e falha

### Para que serve

Serve para diferenciar a origem de um problema, sua manifestação e seu impacto percebido.

### Explicação detalhada e realista

Defeito é uma imperfeição no produto, como código, requisito ou projeto incorreto. Erro pode surgir quando o defeito é executado ou provoca um estado incorreto. Falha é o comportamento externo incorreto percebido pelo usuário ou sistema.

Exemplo: um código que divide por uma variável sem verificar se ela é zero contém um defeito. Quando o usuário informa zero e o programa tenta dividir, ocorre um erro. Se o sistema trava ou mostra resultado inválido, ocorre uma falha.

### Metáfora

Defeito é a rachadura escondida na peça. Erro é a peça cedendo durante o uso. Falha é a máquina parando na frente do operador.

### Situações de uso / exemplo real

Um campo obrigatório sem validação é defeito. Quando o usuário deixa o campo vazio e o sistema processa, ocorre erro. Se o relatório sai incompleto, o usuário observa uma falha.

### Como posso aplicar no dia a dia

Não corrija só a falha visível. Procure o defeito original. Caso contrário, você trata sintomas e não causa.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[10 - Manutenção de Software e Rastreabilidade]]

## Pontos importantes para prova ou revisão

- Qualidade está ligada a requisitos e satisfação do cliente.
- Qualidade pode ser medida, monitorada, gerenciada e melhorada.
- Inspeções podem detectar defeitos antes da execução.
- Checklists ajudam a padronizar revisões.
- O custo de corrigir defeitos aumenta quanto mais tarde eles são descobertos.
- Defeito, erro e falha não são a mesma coisa.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Qualidade | Capacidade de satisfazer requisitos e necessidades |
| Inspeção | Revisão sistemática de artefatos |
| Checklist | Lista de verificação de possíveis problemas |
| Defeito | Imperfeição no produto ou artefato |
| Erro | Estado incorreto gerado a partir de um defeito |
| Falha | Comportamento incorreto percebido |
| Prevenção | Ações para evitar defeitos |
| Avaliação | Ações para detectar defeitos |

## Possíveis notas futuras

- Testes de software
- Revisão técnica formal
- Pair programming
- Qualidade em métodos ágeis
- Garantia da qualidade de software

## Fonte

Material usado como base:

- Nome do arquivo: 04-parte1-Qualidade de Software.pdf
- Tipo do arquivo: PDF
- Matéria: Engenharia de Software I
