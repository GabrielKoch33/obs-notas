---
materia: Engenharia de Software I
tipo: aula
status: refeito_por_ia
fonte:
  - 07-parte1-Requisitos + Gerência de Requisitos.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - requisitos
  - engenharia-de-requisitos
---

# Requisitos de Software e Engenharia de Requisitos

Esta nota explica requisitos funcionais, requisitos não funcionais, regras de negócio e o processo de engenharia de requisitos. Esse assunto é central porque boa parte dos problemas de software começa antes do código: começa quando o problema é mal compreendido.

## Palavras-chave

- Requisitos
- Requisitos funcionais
- Requisitos não funcionais
- [[08 - Modelos de Desenvolvimento|Regras de negócio]]
- [[08 - Modelos de Desenvolvimento|Domínio]]
- Elicitação
- Especificação
- Verificação
- Validação
- Gerência de requisitos
- Rastreabilidade

## Resumo geral da aula

Requisitos expressam propriedades, funções e restrições do software do ponto de vista das necessidades do usuário ou cliente. Levantar requisitos é uma atividade complexa porque envolve comunicação, entendimento do domínio, negociação e validação.

A Engenharia de Requisitos envolve produção e gerência dos requisitos. Produzir requisitos inclui levantar, registrar, verificar e validar. Gerenciar requisitos inclui controlar mudanças, manter rastreabilidade, preservar histórico e garantir que alterações não destruam o escopo do projeto.

---

## 1. O que são requisitos

### Para que serve

Requisitos servem para definir o que o software deve fazer, quais restrições deve respeitar e quais expectativas precisa atender.

### Explicação detalhada e realista

Um requisito é uma descrição de uma função, característica ou restrição do sistema. Ele pode nascer de uma necessidade do usuário, uma [[08 - Modelos de Desenvolvimento|regra de negócio]], uma exigência legal, uma limitação técnica ou uma expectativa de qualidade.

Sem requisitos claros, a equipe corre o risco de construir algo tecnicamente funcional, mas inadequado ao problema. Por isso, requisito não é burocracia: é a base para projeto, implementação, teste, validação e manutenção.

### Metáfora

Requisitos são como as medidas e especificações de uma roupa sob medida. Sem medidas claras, a roupa pode até ser costurada, mas dificilmente servirá bem.

### Situações de uso / exemplo real

Em um sistema médico, “permitir registrar prescrições” é requisito funcional. “Armazenar prontuários por no mínimo 10 anos” pode ser regra/restrição ligada ao negócio ou legislação. “Funcionar em celular e tablet” é requisito não funcional de portabilidade/usabilidade.

### Como posso aplicar no dia a dia

Antes de programar, escreva requisitos numerados. Mesmo simples: RF001, RF002, RNF001. Isso ajuda a testar e rastrear depois.

### Relações com outras notas

- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]
- [[10 - Manutenção de Software e Rastreabilidade]]
- [[08 - Modelos de Desenvolvimento]]

---

## 2. Requisitos funcionais

### Para que serve

Servem para descrever funções que o sistema deve executar.

### Explicação detalhada e realista

Requisitos funcionais dizem o que o software deve fazer. Eles normalmente aparecem como ações do usuário ou do sistema: cadastrar, consultar, emitir, calcular, aprovar, bloquear, excluir, enviar, gerar, importar, exportar.

Um bom requisito funcional deve evitar ambiguidade. “O sistema deve ser rápido” não é funcional e nem mensurável. “O sistema deve emitir relatório de compras por período” é funcional. “O sistema deve responder em até 2 segundos” é não funcional.

### Metáfora

Requisitos funcionais são os verbos do sistema: o que ele faz.

### Situações de uso / exemplo real

RF001 - O sistema deve permitir cadastrar clientes.  
RF002 - O sistema deve calcular gastos mensais.  
RF003 - O sistema deve emitir relatório de compras detalhado por produto.

### Como posso aplicar no dia a dia

Use uma estrutura simples: “O sistema deve permitir [ação] [objeto] [condição, se houver]”.

### Relações com outras notas

- [[06 - Atributos e Características de Qualidade de Software]]
- [[09 - Prototipação, UX, UI e Validação de Ideias]]

---

## 3. Requisitos não funcionais

### Para que serve

Servem para definir qualidades, restrições e condições globais do sistema.

### Explicação detalhada e realista

Requisitos não funcionais descrevem como o sistema deve se comportar ou quais restrições deve obedecer. Eles envolvem desempenho, segurança, usabilidade, manutenibilidade, compatibilidade, portabilidade, confiabilidade, custo, prazo e tecnologias.

Eles são críticos porque muitas vezes determinam a arquitetura. Um sistema que precisa atender milhares de usuários simultâneos será projetado de forma diferente de um sistema usado por uma pessoa.

### Metáfora

Se requisitos funcionais dizem “o que o carro faz”, requisitos não funcionais dizem “com que velocidade, segurança, consumo, conforto e confiabilidade ele faz”.

### Situações de uso / exemplo real

RNF001 - A base de dados deve permitir acesso apenas a usuários autorizados.  
RNF002 - O tempo de resposta não deve ultrapassar 30 segundos.  
RNF003 - O sistema deve funcionar em Android e iOS.

### Como posso aplicar no dia a dia

Sempre pergunte: há restrição de tempo, segurança, ambiente, desempenho, usabilidade, custo ou prazo?

### Relações com outras notas

- [[06 - Atributos e Características de Qualidade de Software]]

---

## 4. Regras de negócio e domínio

### Para que serve

Servem para representar o contexto real onde o software será aplicado.

### Explicação detalhada e realista

Domínio é a área de negócio ou problema específico em que o software atua. Regra de negócio é uma restrição ou política desse domínio. Nem toda regra de negócio é criada pela equipe de software; muitas vêm da empresa, legislação, processo interno ou área profissional.

Confundir regra de negócio com requisito funcional é comum. Uma regra pode dizer “o médico não pode tirar fotos de face e partes íntimas do paciente”. O software deve implementar mecanismos para respeitar essa regra, mas a origem da restrição é o domínio.

### Metáfora

O domínio é o território. As regras de negócio são as leis desse território. O software é a infraestrutura construída para funcionar dentro dele.

### Situações de uso / exemplo real

Em um sistema de estacionamento, a cobrança por hora ou mensalidade é regra de negócio. O requisito funcional pode ser “calcular valor da estadia”.

### Como posso aplicar no dia a dia

Ao modelar um sistema, separe: o que é função do sistema? O que é regra do negócio? O que é restrição técnica?

### Relações com outras notas

- [[01 - Introdução à Engenharia de Software e Problemas Comuns]]
- [[09 - Prototipação, UX, UI e Validação de Ideias]]

---

## 5. Elicitação e especificação

### Para que serve

Servem para descobrir, compreender e formalizar os requisitos.

### Explicação detalhada e realista

Elicitação é o levantamento dos requisitos. Envolve entrevistas, observação, análise de documentos, workshops, protótipos e conversas com stakeholders. É complexa porque usuários podem não saber exatamente o que querem, podem discordar entre si ou podem omitir regras que consideram óbvias.

Especificação é o registro formal dos requisitos. Pode envolver textos, diagramas, tabelas, protótipos, casos de uso e modelos. Uma boa especificação reduz ambiguidade e serve de base para validação, projeto e testes.

### Metáfora

Elicitar é investigar. Especificar é escrever o mapa da investigação de forma que outros possam seguir.

### Situações de uso / exemplo real

O analista entrevista o setor financeiro, descobre regras de aprovação, registra requisitos numerados e cria um protótipo para validar o fluxo.

### Como posso aplicar no dia a dia

Não confie apenas em uma conversa informal. Registre, organize, confirme e peça aceite.

### Relações com outras notas

- [[09 - Prototipação, UX, UI e Validação de Ideias]]

---

## 6. Verificação e validação de requisitos

### Para que serve

Servem para garantir que os requisitos sejam corretos, claros e aceitos.

### Explicação detalhada e realista

Verificação avalia a qualidade dos requisitos: estão claros? Ambíguos? Testáveis? Numerados? Rastreáveis? Têm fonte? Violam escopo? Estão relacionados aos objetivos do sistema?

Validação busca aceite do cliente ou usuário. Um requisito pode estar bem escrito tecnicamente, mas não representar o que o cliente realmente precisa. Por isso, validar é confirmar a necessidade com quem entende do domínio.

### Metáfora

Verificação pergunta: “o requisito está bem escrito?”. Validação pergunta: “esse requisito certo resolve o problema certo?”.

### Situações de uso / exemplo real

Um requisito diz: “o sistema deve ser fácil de usar”. Na verificação, ele falha porque é subjetivo. Na validação, o cliente pode dizer que precisa que novos usuários façam cadastro sem treinamento. O requisito pode ser reescrito com critérios mensuráveis.

### Como posso aplicar no dia a dia

Use checklist. Requisito claro? Testável? Tem fonte? Tem identificador? Está dentro do escopo? Está relacionado ao objetivo?

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

## Pontos importantes para prova ou revisão

- Requisitos expressam funções, propriedades e restrições.
- Requisito funcional descreve o que o sistema faz.
- Requisito não funcional descreve qualidade ou restrição.
- Regra de negócio vem do domínio.
- Engenharia de Requisitos envolve concepção, levantamento, elaboração, negociação, especificação, validação e gestão.
- Verificação avalia qualidade dos requisitos.
- Validação busca aceite do cliente.
- Requisitos devem ser identificados, rastreáveis e testáveis.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| RF | Requisito funcional |
| RNF | Requisito não funcional |
| RN | Regra de negócio |
| Domínio | Área de negócio do sistema |
| Elicitação | Levantamento dos requisitos |
| Especificação | Registro formal dos requisitos |
| Verificação | Avaliação da qualidade do requisito |
| Validação | Aceite do requisito pelo cliente |
| Rastreabilidade | Ligação entre requisito, origem, projeto, teste e implementação |

## Possíveis notas futuras

- Casos de uso
- Histórias de usuário
- Critérios de aceite
- Matriz de rastreabilidade
- Requisitos ágeis

## Fonte

Material usado como base:

- Nome do arquivo: 07-parte1-Requisitos + Gerência de Requisitos.pdf
- Tipo do arquivo: PDF
- Matéria: Engenharia de Software I
