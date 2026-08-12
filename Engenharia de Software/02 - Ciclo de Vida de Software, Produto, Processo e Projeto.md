---
materia: Engenharia de Software I
tipo: aula
status: refeito_por_ia
fonte:
  - 02-parte1-Ciclos de Vida.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - ciclo-de-vida
  - processo
  - projeto
---

# Ciclo de Vida de Software, Produto, Processo e Projeto

Esta nota explica a diferença entre ciclo de vida de produto, processo e projeto. O tema é central porque software não termina no momento em que é implementado: ele nasce, evolui, recebe manutenção, sofre mudanças e pode um dia ser substituído ou descontinuado.

## Palavras-chave

- Ciclo de vida
- Produto
- Projeto
- Processo
- Release
- Versão
- Manutenção
- Maturidade organizacional
- Software sob encomenda
- Produto customizável

## Resumo geral da aula

O ciclo de vida de software descreve as fases pelas quais um software passa desde sua concepção até o fim de seu uso. Ele pode ser analisado sob duas visões: ciclo de vida de produto e ciclo de vida de processo/projeto.

O ciclo de vida de produto acompanha o software durante toda sua existência. O ciclo de vida de processo ou projeto descreve como o software é construído, entregue, versionado e evoluído. Essa distinção é importante porque um software pode ter vários projetos ao longo da vida: projeto inicial, projeto de nova versão, projeto de migração, projeto de manutenção, projeto de integração etc.

---

## 1. Ciclo de vida de produto

### Para que serve

Serve para entender a existência completa de um software: concepção, construção, uso, atualização, manutenção, evolução e retirada de operação.

### Explicação detalhada e realista

Um software raramente termina quando a primeira versão entra em produção. Depois da entrega, surgem correções, novas funcionalidades, mudanças legais, alterações de ambiente, atualização de banco de dados, troca de sistema operacional, novas integrações e melhorias de desempenho.

Essa característica torna software diferente de produtos físicos simples. Um prédio ou uma mesa podem exigir manutenção, mas seu comportamento funcional não muda constantemente. O software, por outro lado, está preso ao ambiente de negócio e tecnológico. Quando o negócio muda, o software precisa acompanhar.

### Metáfora

O ciclo de vida de produto é como a vida de uma cidade. Ela é planejada, construída, habitada, reformada, ampliada e adaptada com o tempo. Não basta inaugurar; é preciso manter ruas, redes, serviços e regras funcionando.

### Situações de uso / exemplo real

Um sistema de folha de pagamento precisa ser atualizado sempre que leis trabalhistas, impostos ou regras sindicais mudam. A primeira entrega não encerra o produto; ela apenas inicia sua vida operacional.

### Como posso aplicar no dia a dia

Ao criar um sistema acadêmico ou pessoal, pense no que pode mudar: campos, regras, usuários, permissões, relatórios, formas de acesso e banco de dados. Projetar pensando em mudança reduz retrabalho.

### Relações com outras notas

- [[10 - Manutenção de Software e Rastreabilidade]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 2. Ciclo de vida de processo/projeto

### Para que serve

Serve para organizar as fases de construção de uma versão, release ou incremento do software.

### Explicação detalhada e realista

O processo é uma receita geral de trabalho. Ele define o que será feito, quando será feito, por quem, com quais insumos e quais resultados serão produzidos. O projeto é a execução concreta dessa receita em um caso específico.

A diferença é importante: o processo pode dizer que toda demanda deve passar por levantamento, análise, implementação, teste e entrega. O projeto é a demanda real: construir o módulo financeiro, criar o app mobile ou migrar o banco de dados.

### Metáfora

O processo é a receita do bolo. O projeto é a preparação daquele bolo em uma cozinha específica, por pessoas específicas, com tempo e ingredientes reais. O produto é o bolo final.

### Situações de uso / exemplo real

Uma empresa pode ter um processo padrão para desenvolver sistemas. Cada cliente, porém, gera um projeto diferente: um sistema para clínica, outro para escola, outro para comércio. O processo organiza; o projeto executa.

### Como posso aplicar no dia a dia

Em trabalhos acadêmicos, defina seu mini-processo: análise do problema, requisitos, modelagem, implementação, testes e entrega. Depois aplique esse processo em cada trabalho como um projeto específico.

### Relações com outras notas

- [[03 - Processos de Software, Atividades Fundamentais, CMMI e MPS.br]]
- [[04 - Modelos de Desenvolvimento de Software - Cascata, Incremental, Iterativo, V, Espiral e Prototipação]]

---

## 3. Processo definido

### Para que serve

Um processo definido serve para reduzir improviso, permitir repetição de boas práticas e tornar o desenvolvimento mais controlável.

### Explicação detalhada e realista

Um processo é considerado definido quando há documentação sobre o produto que será gerado, os procedimentos, os agentes envolvidos, os insumos necessários e os resultados esperados. Sem isso, cada pessoa trabalha de um jeito, e a organização perde previsibilidade.

Isso não significa burocratizar tudo. Um processo útil deve orientar o trabalho sem impedir adaptação. O problema não é ter processo; o problema é ter processo pesado demais, mal comunicado ou ignorado pela equipe.

### Metáfora

Um processo definido é como um checklist de piloto. Ele não substitui a habilidade do piloto, mas reduz a chance de esquecer etapas críticas.

### Situações de uso / exemplo real

Uma empresa sem processo pode aceitar mudanças por WhatsApp, implementar sem análise, testar apenas em produção e documentar depois — ou nunca. Uma empresa com processo define entrada da demanda, análise, aprovação, implementação, teste e registro da mudança.

### Como posso aplicar no dia a dia

Crie checklists simples: requisitos levantados? Escopo definido? Telas desenhadas? Código testado? Alterações registradas? Isso já é uma forma básica de processo.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 4. Releases, versões e evolução

### Para que serve

Serve para entender que software evolui por entregas, não apenas por uma entrega única.

### Explicação detalhada e realista

Uma release é uma entrega organizada de uma versão do software. Essa versão pode conter correções, melhorias, novas funcionalidades ou mudanças internas. Em projetos modernos, releases são essenciais para entregar valor mais cedo e controlar evolução.

Quando uma organização não controla versões, fica difícil saber qual cliente recebeu qual funcionalidade, qual erro foi corrigido, qual requisito foi alterado e qual versão está em produção.

### Metáfora

Versões de software são como edições de um livro técnico. Cada edição pode corrigir erros, adicionar capítulos e atualizar conceitos. Sem controle de edição, ninguém sabe qual conteúdo está lendo.

### Situações de uso / exemplo real

Um aplicativo pode ter a versão 1.0 com login e cadastro, 1.1 com recuperação de senha, 1.2 com relatório e 2.0 com mudança de arquitetura. Cada versão representa um marco de evolução.

### Como posso aplicar no dia a dia

Use Git e changelog em projetos. Mesmo em trabalhos pequenos, registre versões: `v0.1`, `v0.2`, `v1.0`. Isso ajuda a entender sua evolução.

### Relações com outras notas

- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]
- [[10 - Manutenção de Software e Rastreabilidade]]

## Pontos importantes para prova ou revisão

- Ciclo de vida de produto acompanha o software durante toda sua existência.
- Ciclo de vida de processo/projeto descreve como uma versão ou projeto é construído.
- Processo não é produto; processo é a receita, produto é o resultado.
- Software precisa de manutenção porque regras de negócio e tecnologia mudam.
- Releases e versões ajudam a controlar evolução.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Ciclo de vida | Fases pelas quais o software passa |
| Produto | Software como resultado final ou em evolução |
| Processo | Receita organizada de desenvolvimento |
| Projeto | Execução concreta de um processo para atingir um objetivo |
| Release | Entrega organizada de uma versão |
| Versão | Estado identificado de um software em determinado momento |
| Manutenção | Modificação do software após entrega ou entrada em produção |

## Possíveis notas futuras

- Gestão de releases
- Versionamento semântico
- DevOps e ciclo de entrega contínua
- Processo ágil versus processo tradicional

## Fonte

Material usado como base:

- Nome do arquivo: 02-parte1-Ciclos de Vida.pdf
- Tipo do arquivo: PDF
- Matéria: Engenharia de Software I
