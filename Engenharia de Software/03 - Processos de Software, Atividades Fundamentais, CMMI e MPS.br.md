---
materia: Engenharia de Software I
tipo: aula
status: refeito_por_ia
fonte:
  - 03-parte1-Processos+CMMI+MPSbr.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - processos
  - cmmi
  - mpsbr
---

# Processos de Software, Atividades Fundamentais, CMMI e MPS.br

Esta nota explica processos de software como estruturas de trabalho usadas para desenvolver sistemas de forma mais previsível. Também apresenta CMMI e MPS.br como modelos de maturidade voltados à melhoria dos processos organizacionais.

## Palavras-chave

- Processo de software
- Especificação
- Projeto
- Implementação
- Validação
- Evolução
- Modelo de processo
- CMMI
- MPS.br
- Maturidade
- Melhoria contínua

## Resumo geral da aula

Um processo de software é um conjunto estruturado de atividades necessárias para desenvolver e evoluir um sistema. Embora existam diversos processos, muitos compartilham atividades fundamentais: especificação, projeto e implementação, validação e evolução.

Modelos de processo são representações abstratas desses processos. Eles não são a realidade completa de uma empresa, mas ajudam a organizar como o desenvolvimento deve ocorrer. Já CMMI e MPS.br procuram avaliar e melhorar a maturidade dos processos organizacionais.

---

## 1. Processo de software

### Para que serve

Serve para transformar desenvolvimento de software em um trabalho mais organizado, controlável e repetível.

### Explicação detalhada e realista

Sem processo, o desenvolvimento tende a depender de improviso. Cada pessoa decide como levantar requisito, quando testar, como registrar mudança e quando entregar. Isso até pode funcionar em projetos muito pequenos, mas se torna problemático quando há equipe, cliente, prazo, custo, manutenção e qualidade envolvidos.

Um processo não garante sucesso automaticamente, mas reduz incerteza. Ele cria uma base comum para comunicação, planejamento, execução, validação e evolução.

### Metáfora

Processo de software é como a linha de produção adaptável de uma oficina. Não significa que todos os produtos serão iguais, mas que existe uma forma organizada de receber pedidos, produzir, revisar e entregar.

### Situações de uso / exemplo real

Uma empresa pode definir que toda nova funcionalidade passa por análise de requisito, estimativa, aprovação, desenvolvimento, teste e implantação. Esse fluxo evita que mudanças sejam feitas diretamente em produção sem controle.

### Como posso aplicar no dia a dia

Crie um processo mínimo para seus projetos: problema, requisitos, modelagem, implementação, teste e revisão. Com o tempo, adicione versionamento, documentação e checklist.

### Relações com outras notas

- [[02 - Ciclo de Vida de Software, Produto, Processo e Projeto]]
- [[04 - Modelos de Desenvolvimento de Software - Cascata, Incremental, Iterativo, V, Espiral e Prototipação]]

---

## 2. Atividades fundamentais do processo de software

### Para que serve

Servem como blocos básicos presentes na maioria dos processos de desenvolvimento.

### Explicação detalhada e realista

A especificação define o que o sistema deve fazer. O projeto e a implementação definem como o sistema será organizado e construído. A validação verifica se o sistema atende ao que o cliente precisa. A evolução permite adaptar o software a mudanças.

Essas atividades podem aparecer em ordem linear, em ciclos, em incrementos ou misturadas em abordagens ágeis. O importante é perceber que elas sempre existem de alguma forma. Mesmo em um projeto informal, alguém especifica, implementa, testa e muda.

### Metáfora

Essas atividades são como etapas cognitivas de resolver um problema: entender, planejar, executar, conferir e ajustar.

### Situações de uso / exemplo real

No desenvolvimento de um sistema de vendas: especificação define cadastro de produtos e emissão de pedidos; projeto define banco, telas e arquitetura; implementação cria o código; validação testa se as regras funcionam; evolução adiciona promoções, relatórios e integração com nota fiscal.

### Como posso aplicar no dia a dia

Sempre separe mentalmente: ainda estou entendendo o problema ou já estou implementando? Já validei com alguém? O que pode mudar depois? Isso evita começar pelo código sem clareza.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[10 - Manutenção de Software e Rastreabilidade]]

---

## 3. Modelos de processo

### Para que serve

Servem para representar formas diferentes de organizar o desenvolvimento.

### Explicação detalhada e realista

Um modelo de processo não é uma regra universal. Ele é uma representação abstrata de como o desenvolvimento pode ser organizado. Cascata, incremental, iterativo, espiral, prototipação, em V e outros modelos respondem a contextos diferentes.

O erro comum é escolher modelo por moda. A escolha deve considerar risco, clareza dos requisitos, participação do cliente, urgência da entrega, estabilidade do domínio, necessidade de documentação, tamanho da equipe e criticidade do sistema.

### Metáfora

Modelos de processo são como estratégias de viagem. Ir de ônibus, carro, avião ou bicicleta depende de distância, custo, urgência, conforto e rota. Nenhuma estratégia é universalmente melhor.

### Situações de uso / exemplo real

Um sistema bancário crítico pode exigir forte validação, documentação e controle. Um protótipo de app para testar uma ideia pode exigir ciclos rápidos e feedback. O modelo deve respeitar o problema.

### Como posso aplicar no dia a dia

Antes de escolher uma abordagem, pergunte: os requisitos estão claros? O cliente participa? O risco é alto? Posso entregar por partes? Preciso validar cedo?

### Relações com outras notas

- [[04 - Modelos de Desenvolvimento de Software - Cascata, Incremental, Iterativo, V, Espiral e Prototipação]]
- [[09 - Prototipação, UX, UI e Validação de Ideias]]

---

## 4. CMMI

### Para que serve

CMMI serve para orientar a melhoria e maturidade dos processos de uma organização.

### Explicação detalhada e realista

CMMI não é um modelo de desenvolvimento como cascata ou incremental. Ele é um modelo de maturidade e capacidade. Seu foco é avaliar se a organização possui processos estáveis, definidos, gerenciados e melhorados continuamente.

Em uma organização imatura, o sucesso depende muito de esforço individual. Em uma organização mais madura, existem práticas, métricas, padrões, controles e melhoria contínua. Isso não elimina pessoas talentosas, mas reduz dependência de heroísmo.

### Metáfora

CMMI é como avaliar a maturidade de uma academia. Uma academia imatura depende de cada instrutor fazer tudo do próprio jeito. Uma academia madura tem métodos, avaliações, acompanhamento, indicadores e melhoria dos treinos.

### Situações de uso / exemplo real

Uma fábrica de software pode usar CMMI para melhorar estimativas, controle de projetos, qualidade, gestão de requisitos e padronização de processos.

### Como posso aplicar no dia a dia

Mesmo sem certificação, pense em maturidade: seus projetos têm padrão? Você mede progresso? Registra mudanças? Aprende com erros anteriores? Repete boas práticas?

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 5. MPS.br

### Para que serve

MPS.br serve como modelo brasileiro de melhoria de processo de software, especialmente relevante para empresas nacionais.

### Explicação detalhada e realista

O MPS.br propõe níveis de maturidade para orientar a melhoria dos processos. Ele ajuda organizações a evoluírem gradualmente, desde práticas mais básicas de gerência de projetos e requisitos até níveis mais avançados de análise, definição, reutilização, controle quantitativo e otimização.

A ideia central é que processo não melhora por discurso. Melhora com práticas, avaliação, medição e ações contínuas.

### Metáfora

MPS.br é como uma trilha de progressão. A empresa não começa no topo; ela sobe níveis conforme domina práticas essenciais.

### Situações de uso / exemplo real

Uma empresa pequena pode começar estruturando gerência de requisitos e gerência de projetos. Depois pode avançar para garantia da qualidade, medição, configuração e melhoria organizacional.

### Como posso aplicar no dia a dia

Use a lógica de evolução gradual: primeiro organize requisitos e tarefas; depois controle mudanças; depois registre métricas; depois melhore com base nos dados.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

## Pontos importantes para prova ou revisão

- Processo de software é um conjunto estruturado de atividades.
- Atividades fundamentais: especificação, projeto/implementação, validação e evolução.
- Modelo de processo é uma representação abstrata.
- CMMI e MPS.br são modelos de maturidade, não modelos de ciclo de vida.
- Maturidade reduz improviso e dependência de esforço heroico.
- Melhoria de processo é contínua.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Processo de software | Conjunto de atividades para desenvolver e evoluir software |
| Especificação | Definição do que o sistema deve fazer |
| Validação | Verificação se o sistema atende às necessidades do cliente |
| Evolução | Mudanças no software ao longo do tempo |
| CMMI | Modelo de maturidade e capacidade de processos |
| MPS.br | Modelo brasileiro de melhoria de processo de software |
| Maturidade | Grau de estabilidade, controle e melhoria dos processos |

## Possíveis notas futuras

- Scrum e CMMI
- Métricas de processo
- Gestão quantitativa de projetos
- Auditoria de processos

## Fonte

Material usado como base:

- Nome do arquivo: 03-parte1-Processos+CMMI+MPSbr.pdf
- Tipo do arquivo: PDF
- Matéria: Engenharia de Software I
