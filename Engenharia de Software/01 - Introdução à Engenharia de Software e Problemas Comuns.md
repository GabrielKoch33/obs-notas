---
materia: Engenharia de Software I
tipo: aula
status: refeito_por_ia
fonte:
  - 01-parte1-Introdução+Problemas Comuns.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - software
  - processo
---

# Introdução à Engenharia de Software e Problemas Comuns

Esta nota apresenta o papel da Engenharia de Software como disciplina voltada à construção, evolução e manutenção de sistemas complexos. O foco não é apenas “programar”, mas organizar o trabalho para que o software atenda necessidades reais, tenha qualidade, possa ser modificado e não dependa apenas de esforço improvisado.

## Palavras-chave

- Software
- Engenharia de Software
- Processo
- Métodos
- Ferramentas
- Requisitos
- Escopo
- Qualidade
- Manutenção
- Problemas comuns

## Resumo geral da aula

Software é um produto lógico, não físico. Ele não se desgasta como uma peça mecânica, mas pode se tornar defasado quando o ambiente muda, quando as regras de negócio evoluem ou quando novas necessidades surgem. Por isso, construir software exige disciplina: entender o problema, planejar uma solução, modelar, construir, testar, entregar e manter.

A Engenharia de Software surge para reduzir o caos do desenvolvimento. Ela oferece processos, métodos, ferramentas e procedimentos para transformar necessidades em sistemas úteis, dentro de prazos, custos e padrões de qualidade aceitáveis.

---

## 1. O que é software

### Para que serve

Software serve para transformar dados, regras e necessidades humanas em comportamento computacional. Ele automatiza tarefas, apoia decisões, organiza processos e entrega informação útil para pessoas ou organizações.

### Explicação detalhada e realista

Do ponto de vista técnico, software envolve programas, dados, documentação, configurações, modelos, requisitos e demais artefatos que tornam possível a execução e manutenção de um sistema. Do ponto de vista do usuário, porém, o software não é visto como código: ele é uma ferramenta que resolve ou deveria resolver algum problema real.

Essa diferença de visão é essencial. O desenvolvedor tende a enxergar módulos, telas, banco de dados, arquitetura e código. O usuário enxerga resultado: atendimento mais rápido, relatório confiável, cadastro correto, controle financeiro, comunicação eficiente, venda concluída ou tarefa simplificada.

### Metáfora

Software é como uma cozinha de restaurante vista por duas pessoas diferentes. O cliente vê o prato final. O cozinheiro vê ingredientes, equipamentos, processos, tempo de preparo e controle de qualidade. Engenharia de Software é a disciplina que organiza essa cozinha para que o prato seja entregue com consistência, e não por sorte.

### Situações de uso / exemplo real

Em um sistema acadêmico, o usuário quer lançar notas, consultar faltas e emitir histórico. Por trás disso existem regras de aprovação, banco de dados, permissões, integrações, cálculos, relatórios e validações. Se essas partes não forem bem organizadas, o sistema pode até “abrir”, mas entregar resultados errados.

### Como posso aplicar no dia a dia

Ao desenvolver qualquer projeto, mesmo pequeno, pense além do código. Pergunte: qual problema estou resolvendo? Quem usa? Que dados entram? Que resultado sai? O que acontece se a regra mudar? Como vou testar? Como outra pessoa entenderia meu projeto depois?

### Relações com outras notas

- [[02 - Ciclo de Vida de Software, Produto, Processo e Projeto]]
- [[03 - Processos de Software, Atividades Fundamentais, CMMI e MPS.br]]
- [[07 - Requisitos de Software e Engenharia de Requisitos]]

---

## 2. O que é Engenharia de Software

### Para que serve

Engenharia de Software serve para aplicar uma abordagem sistemática, disciplinada e mensurável ao desenvolvimento, operação e manutenção de software.

### Explicação detalhada e realista

A Engenharia de Software não elimina a criatividade do desenvolvimento, mas impede que todo o projeto dependa apenas de intuição. Ela organiza práticas para levantar requisitos, definir escopo, projetar soluções, codificar, testar, validar, implantar e manter sistemas.

Se a programação é uma parte da construção, a Engenharia de Software é o conjunto mais amplo que envolve também análise, comunicação, planejamento, modelagem, qualidade, gestão de mudanças e manutenção. Por isso, um bom engenheiro de software não pensa apenas em “como codar”, mas em como transformar uma necessidade em produto sustentável.

### Metáfora

Programar sem Engenharia de Software é como construir uma casa apenas comprando tijolos e cimento. Engenharia de Software é o projeto arquitetônico, o cronograma, a definição dos materiais, o controle de qualidade e a inspeção da obra.

### Situações de uso / exemplo real

Em uma empresa, um sistema de vendas pode começar simples. Com o tempo, surgem controle de estoque, emissão de nota fiscal, integração com pagamento, relatórios e permissões. Sem Engenharia de Software, cada nova necessidade vira remendo. Com Engenharia de Software, as mudanças são planejadas, rastreadas e testadas.

### Como posso aplicar no dia a dia

Em projetos acadêmicos, use uma estrutura mínima: problema, requisitos, telas ou modelo, código, testes e documentação. Mesmo que o projeto seja pequeno, isso cria hábito profissional.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]
- [[10 - Manutenção de Software e Rastreabilidade]]

---

## 3. Alicerces da Engenharia de Software

### Para que serve

Os alicerces ajudam a separar responsabilidades dentro do desenvolvimento: processo, métodos, ferramentas e procedimentos.

### Explicação detalhada e realista

O processo define o caminho geral: quais atividades serão feitas e em que ordem aproximada. Os métodos explicam como realizar essas atividades, por exemplo, como levantar requisitos, modelar, testar ou revisar. As ferramentas apoiam a execução, como controle de versão, ferramentas CASE, gerenciadores de tarefas, editores, IDEs e sistemas de integração. Os procedimentos conectam tudo isso, definindo padrões, responsabilidades e regras operacionais.

Um erro comum é acreditar que uma ferramenta resolve a ausência de processo. Usar Trello, Jira, Git ou Figma não garante organização se a equipe não sabe o que deve produzir, validar e entregar.

### Metáfora

Processo é a rota da viagem. Métodos são as técnicas de direção. Ferramentas são o carro, o GPS e o painel. Procedimentos são as regras de trânsito e os combinados da equipe.

### Situações de uso / exemplo real

Uma equipe pode usar Git, mas sem regra de branch, revisão e aprovação, o repositório vira um local de conflito. A ferramenta existe, mas o processo e o procedimento são fracos.

### Como posso aplicar no dia a dia

Ao criar projetos, defina um processo simples: levantar requisitos, criar uma versão inicial, testar, revisar, documentar e melhorar. Use ferramentas apenas para apoiar o processo, não para substituí-lo.

### Relações com outras notas

- [[03 - Processos de Software, Atividades Fundamentais, CMMI e MPS.br]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 4. Problemas comuns no desenvolvimento de software

### Para que serve

Estudar problemas comuns ajuda a entender por que projetos falham mesmo quando existem programadores competentes.

### Explicação detalhada e realista

Muitos problemas não nascem no código, mas antes dele: requisitos mal levantados, usuários que não sabem explicar o que precisam, escopo mal definido, divergência entre setores, falta de processo, prazos irreais e custos mal estimados. Quando essas falhas chegam à implementação, o código passa a refletir confusão de negócio.

Outro problema frequente é a distância entre quem constrói e quem usa. Quem desenvolve pode imaginar um fluxo ideal; quem usa conhece exceções, urgências, atalhos e problemas do cotidiano. Se essas visões não são conectadas, o software pode ser tecnicamente correto, mas operacionalmente ruim.

### Metáfora

Um software com requisitos mal definidos é como pedir para alguém construir uma ponte sem informar o tamanho do rio, o peso dos veículos e onde a ponte deve ligar. A construção pode até começar, mas a chance de retrabalho é alta.

### Situações de uso / exemplo real

Um cliente pede “um sistema de cadastro de clientes”. Durante o desenvolvimento, descobre-se que precisa de cadastro de dependentes, histórico de compras, permissões, exportação para Excel, integração com WhatsApp e regras de LGPD. O problema não era apenas cadastro; era gestão de relacionamento com o cliente.

### Como posso aplicar no dia a dia

Antes de programar, escreva perguntas. Quem usa? Para quê? Quais dados são obrigatórios? Quais regras existem? Quais exceções? O que acontece quando algo dá errado? Quanto mais cedo essas dúvidas aparecem, menor o retrabalho.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[09 - Prototipação, UX, UI e Validação de Ideias]]
- [[10 - Manutenção de Software e Rastreabilidade]]

---

## Pontos importantes para prova ou revisão

- Software é produto lógico, não físico.
- Software não se desgasta, mas se torna defasado.
- Engenharia de Software envolve processo, métodos, ferramentas e procedimentos.
- Problemas de requisitos e escopo costumam gerar falhas graves no projeto.
- A prática da Engenharia de Software começa pela compreensão do problema.
- Desenvolvimento de software não é apenas codificação.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Software | Programas, dados, documentos e artefatos que compõem um sistema computacional |
| Engenharia de Software | Aplicação sistemática de processos, métodos e ferramentas ao desenvolvimento e manutenção de software |
| Processo | Conjunto organizado de atividades para construir software |
| Método | Técnica ou prática usada para executar uma etapa do processo |
| Ferramenta | Recurso automatizado ou semiautomatizado que apoia métodos e processos |
| Escopo | Limites do que o sistema deve ou não fazer |
| Requisito | Característica, função ou restrição esperada do software |

## Possíveis notas futuras

- Métodos ágeis
- Padrões de projeto
- Métricas de software
- Pontos de função
- Verificação e validação

## Fonte

Material usado como base:

- Nome do arquivo: 01-parte1-Introdução+Problemas Comuns.pdf
- Tipo do arquivo: PDF
- Matéria: Engenharia de Software I
