---
materia: Engenharia de Software I
tipo: aula
status: refeito_por_ia
fonte:
  - 11-parte1-Manutenção+Rastreabilidade.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - manutencao
  - rastreabilidade
---

# Manutenção de Software e Rastreabilidade

Esta nota explica manutenção de software e rastreabilidade. O tema é central porque software continua mudando após a entrega, e cada mudança precisa ser entendida, controlada e relacionada aos requisitos, projeto e implementação.

## Palavras-chave

- Manutenção de software
- Manutenção corretiva
- Manutenção adaptativa
- Manutenção perfectiva
- Rastreabilidade
- Requisitos
- Impacto
- Dependência
- Matriz de rastreamento

## Resumo geral da aula

A manutenção de software começa logo após o software entrar em produção ou quando o primeiro incremento é disponibilizado. Ela existe porque regras de negócio, necessidades dos clientes, ambiente técnico e expectativas evoluem.

Rastreabilidade é a técnica que relaciona requisitos, projeto e implementação final. Ela permite identificar impactos causados por mudanças nos requisitos e ajuda a manter controle sobre a evolução do sistema.

---

## 1. Manutenção de software

### Para que serve

Serve para adaptar o software após sua entrada em uso.

### Explicação detalhada e realista

Software não termina na primeira entrega. Quando entra em produção, ele passa a interagir com usuários reais, dados reais, regras reais e problemas reais. Isso revela defeitos, limitações, necessidades de adaptação e oportunidades de melhoria.

A manutenção pode ocorrer após a entrada em produção ou após a disponibilização de um incremento. Em modelos incrementais, a manutenção e a evolução podem começar cedo, porque partes do sistema já são usadas enquanto outras ainda estão sendo construídas.

### Metáfora

Manutenção de software é como cuidar de uma estrada em uso. Mesmo depois de inaugurada, ela precisa de reparos, sinalização nova, adaptação ao tráfego e ampliação.

### Situações de uso / exemplo real

Um sistema entra em produção e usuários descobrem que um relatório está calculando impostos incorretamente. A correção é manutenção.

### Como posso aplicar no dia a dia

Ao entregar um projeto, mantenha documentação, controle de versão e lista de mudanças. Isso facilita correções futuras.

### Relações com outras notas

- [[02 - Ciclo de Vida de Software, Produto, Processo e Projeto]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 2. Manutenção corretiva

### Para que serve

Serve para corrigir defeitos encontrados no software.

### Explicação detalhada e realista

Manutenção corretiva ocorre quando o software apresenta comportamento incorreto. Pode envolver erro de cálculo, falha de validação, tela quebrada, regra mal implementada, problema de integração ou inconsistência em dados.

O objetivo é restaurar o comportamento esperado. Porém, corrigir sem investigar causa pode gerar novos defeitos. Por isso, manutenção corretiva precisa de análise de impacto e testes de regressão.

### Metáfora

É como consertar um vazamento. Não basta secar o chão; é preciso achar o cano rompido.

### Situações de uso / exemplo real

A divisão por zero em uma rotina de cálculo é corrigida adicionando validação e tratamento de exceção.

### Como posso aplicar no dia a dia

Ao corrigir bug, escreva o caso que causou a falha e teste se a correção não quebrou outros casos.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]

---

## 3. Manutenção adaptativa

### Para que serve

Serve para adaptar o software a mudanças no ambiente externo.

### Explicação detalhada e realista

Manutenção adaptativa ocorre quando o software precisa acompanhar mudanças fora dele: nova versão do sistema operacional, banco de dados, linguagem, biblioteca, navegador, API, legislação ou infraestrutura.

Nesse caso, o software pode não estar “errado”; o ambiente mudou. A manutenção serve para preservar funcionamento.

### Metáfora

É como trocar o adaptador de tomada quando o padrão elétrico muda. O aparelho continua útil, mas precisa se adaptar ao novo ambiente.

### Situações de uso / exemplo real

Um sistema antigo precisa ser atualizado porque a versão do banco de dados usada será descontinuada.

### Como posso aplicar no dia a dia

Evite dependências sem controle. Documente versões de bibliotecas, banco e ambiente.

### Relações com outras notas

- [[06 - Atributos e Características de Qualidade de Software]]

---

## 4. Manutenção perfectiva

### Para que serve

Serve para melhorar ou adicionar funcionalidades ao software.

### Explicação detalhada e realista

Manutenção perfectiva ocorre quando o sistema recebe novas funções ou melhorias. Ela não corrige necessariamente um defeito, mas amplia valor para o usuário.

É comum em software vivo. Conforme usuários aprendem a usar o sistema, novas ideias aparecem. O desafio é controlar escopo para que melhorias não destruam arquitetura e qualidade.

### Metáfora

É como reformar uma casa para adicionar um escritório. A casa já funcionava, mas agora atende melhor uma nova necessidade.

### Situações de uso / exemplo real

Adicionar exportação para Excel em um relatório já existente é manutenção perfectiva.

### Como posso aplicar no dia a dia

Registre melhorias como requisitos novos, avalie impacto e teste funcionalidades afetadas.

### Relações com outras notas

- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 5. Rastreabilidade

### Para que serve

Serve para relacionar requisitos, projeto, implementação, testes e mudanças.

### Explicação detalhada e realista

Rastreabilidade permite saber de onde veio um requisito, quais características ele atende, quais módulos são afetados, quais interfaces dependem dele e quais outros requisitos estão relacionados.

Sem rastreabilidade, mudanças viram apostas. A equipe altera um requisito sem saber que ele afeta outro módulo, uma tela, um relatório ou uma integração. Com rastreabilidade, é possível estimar impacto e reduzir risco.

### Metáfora

Rastreabilidade é como mapa de fios de uma instalação elétrica. Sem o mapa, mexer em uma tomada pode desligar algo inesperado.

### Situações de uso / exemplo real

Se o requisito RF010 muda, a matriz de rastreabilidade mostra que ele afeta o módulo financeiro, a interface de pagamento, o relatório mensal e o teste CT015.

### Como posso aplicar no dia a dia

Crie tabelas simples ligando requisitos a telas, módulos, testes e fontes. Mesmo uma planilha já ajuda.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 6. Tipos de tabelas de rastreamento

### Para que serve

Servem para organizar relações entre requisitos e outros elementos do projeto.

### Explicação detalhada e realista

A rastreabilidade pode ser organizada por características, necessidades, fontes, dependências, subsistemas e interfaces.

Uma tabela de características relaciona requisitos a características do sistema. Uma tabela de necessidades liga requisitos a problemas de negócio. Uma tabela de fontes indica quem originou cada requisito. Uma tabela de dependência mostra requisitos relacionados. Uma tabela de subsistemas mostra módulos afetados. Uma tabela de interface aponta telas, APIs ou integrações envolvidas.

### Metáfora

Cada tabela é uma lente diferente sobre o mesmo sistema. Uma mostra origem, outra mostra impacto, outra mostra módulos, outra mostra dependências.

### Situações de uso / exemplo real

Para o RF001 “cadastrar cliente”, a fonte pode ser o setor comercial, a necessidade pode ser controlar compradores, o subsistema pode ser CRM, e a interface pode ser Tela de Cadastro de Cliente.

### Como posso aplicar no dia a dia

Em projetos pequenos, faça pelo menos: requisito, fonte, módulo, tela, teste e dependências.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]

## Pontos importantes para prova ou revisão

- Manutenção começa após produção ou após primeiro incremento.
- Manutenção corretiva corrige defeitos.
- Manutenção adaptativa acompanha mudanças do ambiente externo.
- Manutenção perfectiva adiciona ou melhora funcionalidades.
- Rastreabilidade relaciona requisitos, projeto e implementação.
- Rastreabilidade ajuda a identificar impacto de mudanças.
- Tabelas de rastreamento podem ligar requisitos a fontes, necessidades, características, dependências, subsistemas e interfaces.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Manutenção corretiva | Correção de defeitos |
| Manutenção adaptativa | Adaptação a mudanças externas |
| Manutenção perfectiva | Inclusão de funcionalidades ou melhorias |
| Rastreabilidade | Ligação entre requisitos e outros artefatos |
| Matriz de rastreabilidade | Tabela que relaciona requisitos e impactos |
| Impacto | Consequência de uma mudança no sistema |
| Fonte do requisito | Origem do requisito |

## Possíveis notas futuras

- Teste de regressão
- Matriz de rastreabilidade
- Gestão de mudanças em manutenção
- Dívida técnica
- Refatoração

## Fonte

Material usado como base:

- Nome do arquivo: 11-parte1-Manutenção+Rastreabilidade.pdf
- Tipo do arquivo: PDF
- Matéria: Engenharia de Software I
