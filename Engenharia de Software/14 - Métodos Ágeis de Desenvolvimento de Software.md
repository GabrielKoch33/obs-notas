---
materia: Engenharia de Software I
aula: 16
tags:
  - engenharia-de-software
  - métodos-ágeis
  - scrum
  - xp
  - extreme-programming
  - desenvolvimento-ágil
---

## Introdução

Os métodos ágeis surgiram como uma alternativa aos processos tradicionais de desenvolvimento de software, que frequentemente eram considerados excessivamente burocráticos, lentos e pouco adaptáveis às mudanças. A proposta principal dos métodos ágeis é desenvolver software de forma incremental, colaborativa e flexível, entregando valor ao cliente continuamente ao longo do projeto.

Em vez de tentar definir todos os requisitos e planejar todo o desenvolvimento logo no início, os métodos ágeis aceitam que mudanças são inevitáveis e utilizam ciclos curtos de desenvolvimento para adaptar o produto às necessidades reais dos usuários.

## Palavras-chave

Métodos Ágeis, Manifesto Ágil, Scrum, Sprint, Product Backlog, XP, Extreme Programming, Integração Contínua, TDD, Refatoração, Desenvolvimento Incremental, Cliente, Equipe.

---

# O que são Métodos Ágeis

## Para que servem

Os métodos ágeis servem para desenvolver software de forma mais rápida, flexível e alinhada às necessidades do cliente.

Seu objetivo é:

- Adaptar-se facilmente a mudanças;
- Entregar funcionalidades com frequência;
- Melhorar a comunicação entre equipe e cliente;
- Reduzir riscos durante o desenvolvimento;
- Aumentar a qualidade do software.

## Explicação técnica

Nos modelos tradicionais, grande parte do esforço é concentrada no planejamento inicial e na documentação.

Já os métodos ágeis adotam uma abordagem iterativa e incremental, na qual o sistema é desenvolvido em pequenas partes chamadas incrementos.

Cada incremento adiciona novas funcionalidades ao sistema e pode ser avaliado pelo cliente antes da próxima etapa do desenvolvimento.

Essa abordagem permite detectar problemas mais cedo e adaptar o produto às mudanças de requisitos sem comprometer todo o projeto.

## Metáfora

Imagine construir uma casa e mostrar o resultado apenas quando tudo estiver pronto.

Se o cliente não gostar de algo, a correção será cara e demorada.

Os métodos ágeis funcionam de maneira diferente: a casa é construída por partes, e o cliente acompanha constantemente o progresso, podendo sugerir mudanças ao longo da construção.

## Situação de uso / Exemplo real

Uma startup está desenvolvendo um aplicativo de delivery.

Durante o desenvolvimento surgem novas necessidades dos usuários e mudanças de mercado.

Utilizando métodos ágeis, a equipe consegue adaptar rapidamente o sistema sem precisar reiniciar todo o planejamento do projeto.

## Aplicação no dia a dia

O pensamento ágil pode ser aplicado em:

- Organização de estudos;
- Desenvolvimento de projetos pessoais;
- Planejamento de trabalhos acadêmicos;
- Gestão de equipes;
- Desenvolvimento de software.

---

# Manifesto Ágil

## Para que serve

O Manifesto Ágil estabelece os princípios fundamentais que orientam os métodos ágeis.

Ele não define um processo específico, mas apresenta valores que servem como base para diversas metodologias ágeis.

## Explicação técnica

O Manifesto Ágil valoriza:

### Indivíduos e interações

Mais importantes que processos e ferramentas.

A comunicação eficiente entre pessoas é considerada fundamental para o sucesso do projeto.

### Software funcionando

Mais importante que documentação extensa.

A prioridade é entregar software que realmente funcione.

### Colaboração com o cliente

Mais importante que negociações contratuais rígidas.

O cliente participa continuamente do desenvolvimento.

### Resposta a mudanças

Mais importante que seguir um plano fixo.

Mudanças são tratadas como oportunidades de melhoria e não como problemas.

## Importância

Esses valores influenciam praticamente todas as práticas dos métodos ágeis modernos.

---

# Scrum

## Para que serve

O Scrum é um framework de gerenciamento de projetos utilizado para organizar e controlar o desenvolvimento de software em ambientes ágeis. 

Seu objetivo é permitir entregas frequentes e facilitar a adaptação do projeto às mudanças.

## Explicação técnica

O Scrum organiza o trabalho em ciclos chamados Sprints.

Cada Sprint possui duração fixa e produz um incremento funcional do sistema. 

Ao final de cada Sprint, existe uma nova versão do produto contendo funcionalidades concluídas e testadas.

### Product Backlog

É uma lista priorizada contendo todas as funcionalidades desejadas para o sistema.

O backlog é constantemente atualizado conforme novas necessidades surgem.

### Sprint Backlog

Representa o conjunto de tarefas selecionadas para uma Sprint específica.

### Sprint

Período de trabalho com duração fixa durante o qual uma parte do sistema é desenvolvida.

### Incremento

Resultado produzido ao final de uma Sprint.

Consiste em uma versão funcional do software.

## Principais papéis

### Product Owner

Representa os interesses do cliente.

Define prioridades e gerencia o Product Backlog.

### Scrum Master

Ajuda a equipe a seguir os princípios do Scrum.

Remove impedimentos e facilita o processo.

### Equipe de Desenvolvimento

Responsável pela implementação das funcionalidades.

## Metáfora

O Scrum funciona como um campeonato dividido em rodadas.

Ao final de cada rodada existe um resultado concreto que pode ser avaliado antes do início da próxima etapa.

## Situação de uso / Exemplo real

Uma empresa desenvolve um sistema de gestão empresarial.

Em vez de esperar meses pela entrega final, funcionalidades são liberadas gradualmente em Sprints, permitindo que os usuários utilizem o sistema enquanto ele continua evoluindo.

---

# Extreme Programming (XP)

## Para que serve

A Programação Extrema (XP) é um método ágil focado principalmente na qualidade do código e na eficiência do desenvolvimento.

Seu objetivo é produzir software de alta qualidade por meio de práticas técnicas rigorosas.

## Explicação técnica

O XP enfatiza:

- Comunicação constante;
- Feedback rápido;
- Simplicidade;
- Coragem para modificar o código;
- Respeito entre os membros da equipe.

Além disso, utiliza diversas práticas técnicas para melhorar a qualidade do software.

---

# Desenvolvimento Orientado a Testes (TDD)

## Para que serve

O TDD (Test-Driven Development) busca aumentar a qualidade do software e reduzir defeitos.

É considerado uma das práticas mais importantes do XP. 

## Explicação técnica

A principal característica do TDD é que os testes são escritos antes da implementação da funcionalidade.

O ciclo normalmente segue três etapas:

### 1. Criar o teste

Primeiro é criado um teste automatizado para a funcionalidade desejada.

Como a funcionalidade ainda não existe, o teste falha.

### 2. Implementar a solução

É escrito apenas o código necessário para fazer o teste passar.

### 3. Refatorar

O código é melhorado sem alterar seu comportamento.

Após isso, os testes são executados novamente.

## Benefícios

- Menor quantidade de defeitos;
- Maior segurança para alterações;
- Melhor manutenção;
- Código mais confiável.

## Situação real

Antes de implementar uma função de cálculo de desconto, o desenvolvedor cria testes verificando diversos cenários.

Somente depois a implementação é realizada.

---

# Refatoração

## Para que serve

Refatoração é o processo de melhorar a estrutura interna do código sem alterar seu comportamento externo.

## Explicação técnica

Durante a evolução de um sistema, o código pode se tornar:

- Duplicado;
- Confuso;
- Difícil de manter.

A refatoração busca corrigir esses problemas mantendo todas as funcionalidades existentes.

Normalmente ela é realizada juntamente com testes automatizados, garantindo que nenhuma funcionalidade seja quebrada.

## Metáfora

É semelhante a reformar uma casa sem alterar sua finalidade.

A estrutura interna é melhorada, mas a casa continua funcionando normalmente.

---

# Integração Contínua

## Para que serve

A integração contínua busca detectar problemas rapidamente durante o desenvolvimento.

## Explicação técnica

Cada alteração realizada pelos desenvolvedores é integrada frequentemente ao sistema principal.

Após cada integração são executados testes automatizados para verificar se a mudança introduziu defeitos.

Essa prática reduz:

- Conflitos de código;
- Problemas de integração;
- Erros acumulados.

No XP, todos os testes devem ser executados com sucesso sempre que um incremento for integrado ao sistema. 

## Situação real

Uma equipe com dez desenvolvedores realiza integrações diariamente.

Problemas são identificados imediatamente, evitando que erros permaneçam ocultos por semanas.

---

# Escalamento de Métodos Ágeis para Grandes Sistemas

## Para que serve

O escalamento busca adaptar práticas ágeis para projetos de grande porte envolvendo múltiplas equipes e sistemas complexos. 

## Explicação técnica

Embora os métodos ágeis funcionem muito bem em equipes menores, sua aplicação em grandes projetos apresenta desafios adicionais.

Mesmo em projetos grandes, é importante manter fundamentos ágeis como: 

- Planejamento flexível;
- Releases frequentes;
- Integração contínua;
- Desenvolvimento orientado a testes;
- Comunicação eficiente.

Porém alguns ajustes tornam-se necessários.

### Maior necessidade de documentação

Em projetos extensos, apenas o código não é suficiente.

É necessário produzir documentação adicional para facilitar a comunicação entre equipes. 

### Comunicação entre equipes

Quando existem várias equipes trabalhando simultaneamente, mecanismos formais de comunicação tornam-se essenciais. 

Podem ser utilizados:

- Reuniões frequentes;
- Videoconferências;
- Ferramentas colaborativas;
- Comunicação interequipes.

### Limitações da integração contínua

Em sistemas muito grandes, reconstruir todo o sistema após cada alteração pode ser impraticável.

Mesmo assim, continua sendo importante manter builds frequentes e liberações regulares do software.
### Resistência organizacional

Grandes organizações frequentemente possuem:

- Processos burocráticos;
- Padrões rígidos;
- Estruturas hierárquicas complexas.

Essas características podem dificultar a adoção de métodos ágeis. }

Além disso, equipes podem apresentar diferentes níveis de experiência e existir resistência cultural à mudança. 

---

# Relações com outras notas

- [[03 - Processos de Software, Atividades Fundamentais, CMMI e MPS.br]]
- [[04 - Modelos de Desenvolvimento de Software - Cascata, Incremental, Iterativo, V, Espiral e Prototipação]]
- [[11 - Planejamento e Gerenciamento de Projetos em Software]]
- [[14 - Métricas, Estimativas de Custos e Análise de Viabilidade]]
- [[15 - Estudo de Viabilidade de Software]]

## Resumo Final

Os métodos ágeis surgiram para tornar o desenvolvimento de software mais adaptável às mudanças e mais próximo das necessidades dos usuários. O Manifesto Ágil estabelece valores baseados em colaboração, software funcionando e adaptação contínua. Entre os métodos mais importantes destacam-se o Scrum, focado no gerenciamento de projetos por meio de Sprints, e o XP, focado em práticas técnicas como TDD, refatoração e integração contínua. Embora sejam extremamente eficazes em equipes menores, sua aplicação em sistemas de grande porte exige adaptações relacionadas à documentação, comunicação e coordenação entre múltiplas equipes.