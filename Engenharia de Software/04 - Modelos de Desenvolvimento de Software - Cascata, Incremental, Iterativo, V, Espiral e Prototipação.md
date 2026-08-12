---
materia: Engenharia de Software I
tipo: nota-conceitual
status: criado_por_ia
fonte:
  - 01-parte1-Introdução+Problemas Comuns.pdf
  - 03-parte1-Processos+CMMI+MPSbr.pdf
  - Fundamentos de Sistemas de Informação - Aula 7.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - modelos-de-desenvolvimento
  - ciclo-de-vida
---

# Modelos de Desenvolvimento de Software - Cascata, Incremental, Iterativo, V, Espiral e Prototipação

Esta nota aprofunda os principais modelos de desenvolvimento de software. Ela foi criada separadamente porque os modelos de processo são um dos assuntos estruturais de Engenharia de Software: eles explicam como organizar o trabalho, como lidar com requisitos, como entregar valor e como controlar riscos.

## Palavras-chave

- Modelo cascata
- Modelo incremental
- Modelo iterativo
- Iterativo-incremental
- Prototipação
- Modelo espiral
- Modelo em V
- RAD
- Construir e corrigir
- Risco
- Validação
- Verificação

## Resumo geral da aula

Modelos de desenvolvimento de software são formas de organizar as atividades do processo de software. Eles orientam quando levantar requisitos, quando projetar, quando implementar, quando testar, quando entregar e como lidar com mudanças.

Nenhum modelo é perfeito para todos os casos. O modelo escolhido depende de fatores como clareza dos requisitos, participação do cliente, risco técnico, criticidade do sistema, tamanho do projeto, necessidade de documentação, prazo e maturidade da equipe.

---

## 1. Modelo Cascata

### Para que serve

Serve para organizar o desenvolvimento em fases sequenciais, em que uma etapa depende da conclusão da anterior.

### Explicação detalhada e realista

O modelo cascata, também chamado de clássico, segue uma lógica linear: levantamento de requisitos, análise, projeto, implementação, testes, entrega e manutenção. Ele parte da ideia de que é possível compreender bem o problema antes de construir a solução.

Sua vantagem é a clareza: cada fase possui objetivos e documentos definidos. Isso facilita controle, planejamento e acompanhamento formal. Porém, seu ponto fraco é a rigidez. Projetos reais raramente seguem um fluxo totalmente sequencial, e clientes frequentemente descobrem novas necessidades ao ver partes do sistema funcionando.

O cascata é problemático quando os requisitos são incertos, quando o usuário não sabe explicar o que deseja ou quando o domínio muda muito. Nesses casos, a equipe pode gastar muito tempo produzindo documentação e projeto para algo que precisará ser alterado.

### Metáfora

O modelo cascata é como construir uma ponte: primeiro projeto estrutural, depois fundação, depois pilares, depois pista, depois acabamento. Não faz sentido colocar o asfalto antes dos pilares. O problema é que software nem sempre se comporta como uma ponte; muitas vezes, o cliente só entende o que quer ao ver uma primeira versão funcionando.

### Situações de uso / exemplo real

Pode fazer sentido em sistemas com requisitos estáveis, forte regulação, documentação exigida e pouca tolerância a mudanças informais, como sistemas embarcados, sistemas governamentais muito formalizados ou partes críticas de sistemas industriais.

### Como posso aplicar no dia a dia

Use a lógica do cascata quando você precisa organizar um projeto com etapas bem definidas. Mesmo em projetos pessoais, ele ajuda a lembrar que não se deve codar antes de entender minimamente o problema.

### Relações com outras notas

- [[02 - Ciclo de Vida de Software, Produto, Processo e Projeto]]
- [[03 - Processos de Software, Atividades Fundamentais, CMMI e MPS.br]]

---

## 2. Modelo Iterativo

### Para que serve

Serve para desenvolver o software por ciclos sucessivos, revisando e melhorando a solução a cada iteração.

### Explicação detalhada e realista

No modelo iterativo, o sistema é desenvolvido em repetidas passagens. Cada ciclo revisita atividades como análise, projeto, implementação e teste. A ideia é aprender progressivamente: a primeira versão pode não estar completa, mas ajuda a entender melhor o problema.

O modelo puramente iterativo pode produzir liberações intermediárias, mas nem sempre cada liberação entrega uma parte plenamente utilizável do sistema ao usuário. Muitas vezes, o sistema só se torna completo ao final, ainda que tenha sido refinado em ciclos.

### Metáfora

É como escrever uma redação por versões: rascunho, revisão, nova versão, nova revisão e versão final. Cada ciclo melhora o resultado.

### Situações de uso / exemplo real

Em um sistema acadêmico, a equipe pode primeiro modelar o fluxo de matrícula, depois revisar com usuários, depois melhorar regras, depois ajustar telas e só depois liberar a versão final.

### Como posso aplicar no dia a dia

Ao estudar ou programar, faça versões. Primeiro crie uma solução funcional simples; depois revise, refatore, melhore nomes, valide regras e incremente qualidade.

### Relações com outras notas

- [[09 - Prototipação, UX, UI e Validação de Ideias]]
- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]

---

## 3. Modelo Incremental

### Para que serve

Serve para entregar o sistema por partes utilizáveis, chamadas incrementos.

### Explicação detalhada e realista

No modelo incremental, cada entrega adiciona uma parte funcional ao sistema. Diferente do iterativo puro, o incremento geralmente já entrega valor prático para o usuário. Por exemplo, primeiro entrega cadastro, depois pedidos, depois relatórios, depois integração com pagamento.

Esse modelo é útil porque o cliente começa a usar partes do sistema mais cedo. Também permite feedback real, reduzindo o risco de descobrir tarde demais que a solução não atende ao usuário.

O cuidado é que muitos incrementos adicionados sem arquitetura adequada podem degradar a estrutura do sistema. Se cada entrega for apenas “encaixada” sem planejamento, a manutenção fica cada vez mais cara.

### Metáfora

É como construir uma casa por cômodos utilizáveis. Primeiro um quarto e banheiro funcionais, depois cozinha, depois sala, depois garagem. A casa cresce, mas cada parte precisa respeitar a estrutura geral.

### Situações de uso / exemplo real

Um sistema de e-commerce pode ser entregue em incrementos: catálogo de produtos, carrinho, login, pagamento, rastreamento e relatórios administrativos.

### Como posso aplicar no dia a dia

Divida projetos em entregas pequenas e funcionais. Em vez de tentar fazer tudo de uma vez, entregue primeiro o núcleo útil.

### Relações com outras notas

- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]
- [[10 - Manutenção de Software e Rastreabilidade]]

---

## 4. Modelo Iterativo-Incremental

### Para que serve

Serve para combinar ciclos de melhoria com entregas progressivas de funcionalidades.

### Explicação detalhada e realista

O modelo iterativo-incremental combina duas ideias: repetir ciclos de desenvolvimento e entregar partes do sistema ao longo do tempo. Cada ciclo pode produzir um incremento novo ou melhorar incrementos existentes.

Ele é muito próximo da lógica usada em várias abordagens modernas. O sistema começa com um núcleo e evolui por ciclos. A cada ciclo, a equipe aprende mais, corrige problemas, ajusta requisitos e entrega valor de forma testável e utilizável.

Esse modelo exige um número razoável de requisitos definidos para orientar o núcleo inicial, mas não exige que tudo esteja completamente fechado desde o início.

### Metáfora

É como desenvolver um jogo em versões: primeiro o personagem anda, depois pula, depois interage com objetos, depois recebe inimigos, depois fases, depois ajustes de dificuldade. Cada versão funciona melhor que a anterior e adiciona algo.

### Situações de uso / exemplo real

Um sistema de controle financeiro pode começar com lançamento de despesas, depois relatórios simples, depois categorias, depois gráficos, depois integração bancária.

### Como posso aplicar no dia a dia

Crie MVPs acadêmicos: primeiro a versão mínima funcional, depois melhorias planejadas. Isso ajuda a evitar projetos enormes que nunca ficam prontos.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[09 - Prototipação, UX, UI e Validação de Ideias]]

---

## 5. Prototipação

### Para que serve

Serve para visualizar, testar, comunicar e validar ideias antes da construção definitiva.

### Explicação detalhada e realista

A prototipação cria uma versão inicial, parcial ou simulada do sistema. Pode ser usada para entender requisitos, testar alternativas de interface, validar fluxos, discutir regras e reduzir ambiguidades.

Existem dois tipos importantes. O protótipo descartável é feito rapidamente para aprender e depois é descartado. O protótipo evolucionário já nasce com intenção de evoluir para partes do produto final.

O risco da prototipação é o cliente confundir protótipo com sistema pronto. Uma tela bonita não significa que banco de dados, segurança, validações, arquitetura, testes e regras internas estão completos.

### Metáfora

Protótipo é como uma maquete de prédio. Ela ajuda a visualizar, discutir e corrigir ideias, mas ninguém pode morar dentro dela.

### Situações de uso / exemplo real

Antes de construir uma tela de venda, a equipe desenha um protótipo com campos de cliente, produtos, desconto, forma de pagamento e local de entrega. O usuário avalia se o fluxo faz sentido antes da implementação.

### Como posso aplicar no dia a dia

Antes de codar telas, desenhe em papel, Figma, draw.io ou outra ferramenta. Isso economiza tempo e revela problemas cedo.

### Relações com outras notas

- [[09 - Prototipação, UX, UI e Validação de Ideias]]
- [[07 - Requisitos de Software e Engenharia de Requisitos]]

---

## 6. Modelo Espiral

### Para que serve

Serve para conduzir projetos com ciclos orientados a risco.

### Explicação detalhada e realista

O modelo espiral, associado a Boehm, combina características iterativas da prototipação com controles mais sistemáticos. Cada volta da espiral representa uma fase ou ciclo do projeto. Em cada ciclo, objetivos são definidos, riscos são analisados, alternativas são avaliadas, desenvolvimento/validação ocorre e o próximo ciclo é planejado.

A grande diferença do espiral é o tratamento explícito do risco. Ele é útil quando há incertezas técnicas, alto custo de erro, tecnologias novas ou requisitos difíceis de estabilizar.

### Metáfora

É como explorar uma montanha desconhecida em círculos cada vez mais altos. A cada volta, você avalia o terreno, identifica perigos, corrige rota e sobe mais um nível.

### Situações de uso / exemplo real

Um sistema crítico com integração a tecnologias novas pode usar espiral para validar riscos antes de investir no produto completo: desempenho, segurança, integração, usabilidade e viabilidade técnica.

### Como posso aplicar no dia a dia

Em projetos difíceis, liste riscos antes de começar: “não sei usar essa API”, “não sei se o banco aguenta”, “não sei se o usuário aceitará essa interface”. Ataque os maiores riscos primeiro com pequenos testes.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 7. Modelo em V

### Para que serve

Serve para relacionar fases de desenvolvimento com fases correspondentes de verificação e validação.

### Explicação detalhada e realista

O modelo em V enfatiza que as atividades de teste e validação não devem ser pensadas apenas no final. Cada etapa de concepção tem uma etapa correspondente de verificação ou validação. Requisitos se conectam a testes de aceitação; projeto de sistema se conecta a testes de sistema; projeto de módulos se conecta a testes de integração e unidade.

A força do modelo em V está em deixar claro que qualidade deve ser planejada desde o início. Ele é útil quando há necessidade de rastreabilidade entre requisitos, projeto, implementação e testes.

### Metáfora

O modelo em V é como planejar uma prova antes de ensinar o conteúdo. Ao definir o que será ensinado, você já pensa em como comprovar que foi aprendido.

### Situações de uso / exemplo real

Em sistemas que precisam comprovar conformidade, como aplicações médicas, financeiras ou industriais, o modelo em V ajuda a ligar cada requisito a testes correspondentes.

### Como posso aplicar no dia a dia

Ao escrever um requisito, já pense: como vou testar isso? O requisito é verificável? Qual evidência mostra que ele foi atendido?

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[10 - Manutenção de Software e Rastreabilidade]]

---

## 8. RAD

### Para que serve

Serve para acelerar o desenvolvimento por meio de ciclos curtos, forte reaproveitamento e foco em entrega rápida.

### Explicação detalhada e realista

RAD, ou Rapid Application Development, prioriza velocidade de entrega. Normalmente envolve prototipação, ferramentas visuais, componentes reutilizáveis e participação intensa do usuário.

O RAD pode ser útil quando o sistema tem escopo bem delimitado e pode ser construído rapidamente. Porém, pode ser arriscado em sistemas muito complexos, críticos ou com arquitetura difícil.

### Metáfora

RAD é como montar um móvel modular com peças prontas. A entrega é rápida, desde que o problema caiba bem nas peças disponíveis.

### Situações de uso / exemplo real

Aplicações administrativas internas simples, painéis, sistemas CRUD e protótipos funcionais podem se beneficiar de RAD.

### Como posso aplicar no dia a dia

Use frameworks e ferramentas que acelerem tarefas repetitivas, mas sem ignorar requisitos, segurança e manutenção.

### Relações com outras notas

- [[09 - Prototipação, UX, UI e Validação de Ideias]]
- [[03 - Processos de Software, Atividades Fundamentais, CMMI e MPS.br]]

---

## 9. Construir e corrigir

### Para que serve

Na prática, não deveria servir como modelo profissional principal, mas aparece em muitas empresas e projetos pequenos.

### Explicação detalhada e realista

Construir e corrigir é uma abordagem caótica: implementa-se algo, usa-se, encontra-se problema, corrige-se, muda-se, remenda-se e continua. Pode funcionar em microprojetos, mas tende a gerar software difícil de manter.

Seu problema é a ausência de planejamento, arquitetura e controle. O sistema cresce por remendos, a documentação não acompanha, e cada mudança fica mais arriscada.

### Metáfora

É como construir uma casa sem planta: levanta uma parede, quebra, muda a porta, puxa um fio, remenda o teto. Pode virar abrigo, mas dificilmente será uma construção segura e sustentável.

### Situações de uso / exemplo real

Scripts pessoais, protótipos descartáveis e automações muito pequenas podem sobreviver com essa abordagem. Sistemas empresariais, não.

### Como posso aplicar no dia a dia

Evite transformar protótipos improvisados em sistemas definitivos sem refatoração, documentação e testes.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[10 - Manutenção de Software e Rastreabilidade]]

## Comparação direta entre modelos

| Modelo | Melhor quando | Principal risco |
|---|---|---|
| Cascata | Requisitos estáveis e forte documentação | Rigidez diante de mudanças |
| Iterativo | É necessário aprender e revisar em ciclos | Pode demorar para entregar algo utilizável |
| Incremental | É possível entregar partes úteis do sistema | Arquitetura pode degradar se mal planejada |
| Iterativo-incremental | Há necessidade de ciclos e entregas parciais | Exige gestão constante de escopo |
| Prototipação | Requisitos ou interface ainda são incertos | Cliente confundir protótipo com produto final |
| Espiral | Riscos técnicos ou de negócio são altos | Pode ser complexo e caro para projetos simples |
| Modelo em V | Testes e rastreabilidade são críticos | Pode ficar rígido se usado de forma burocrática |
| RAD | Prazo curto e escopo bem delimitado | Pode gerar baixa qualidade se acelerar demais |
| Construir e corrigir | Microprojetos ou experimentos rápidos | Caos, retrabalho e manutenção difícil |

## Pontos importantes para prova ou revisão

- Cascata é sequencial e funciona melhor com requisitos estáveis.
- Incremental entrega partes utilizáveis do sistema.
- Iterativo melhora a solução por ciclos.
- Iterativo-incremental combina ciclos e entregas progressivas.
- Prototipação ajuda a elicitar e validar requisitos.
- Espiral é orientado a riscos.
- Modelo em V relaciona desenvolvimento com verificação e validação.
- Construir e corrigir é comum, mas perigoso em projetos maiores.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Cascata | Modelo linear e sequencial |
| Incremento | Parte funcional entregue ao usuário |
| Iteração | Ciclo de trabalho, revisão e melhoria |
| Protótipo | Versão inicial usada para aprender, validar ou demonstrar |
| Risco | Incerteza que pode prejudicar custo, prazo, qualidade ou viabilidade |
| Verificação | Confirma se o produto foi construído corretamente |
| Validação | Confirma se o produto atende à necessidade correta |
| RAD | Desenvolvimento rápido de aplicações |

## Possíveis notas futuras

- Scrum
- Extreme Programming
- RUP
- DevOps
- MVP
- Kanban
- Testes no modelo em V

## Fonte

Materiais usados como base:

- 01-parte1-Introdução+Problemas Comuns.pdf
- 03-parte1-Processos+CMMI+MPSbr.pdf
- Fundamentos de Sistemas de Informação - Aula 7.pdf
