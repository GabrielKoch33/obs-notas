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
  - atributos-de-qualidade
---

# Atributos e Características de Qualidade de Software

Esta nota detalha os atributos de qualidade de software, como funcionalidade, [[12 - Introdução à Segurança da Informação|segurança]], manutenibilidade, usabilidade, confiabilidade, eficiência e portabilidade. Esses atributos ajudam a transformar “software bom” em critérios observáveis e testáveis.

## Palavras-chave

- Funcionalidade
- [[12 - Introdução à Segurança da Informação|Segurança]]
- Acurácia
- Interoperabilidade
- [[10 - Manutenção de Software e Rastreabilidade|Manutenibilidade]]
- Usabilidade
- Confiabilidade
- Eficiência
- Portabilidade
- Testabilidade
- Adaptabilidade

## Resumo geral da aula

Qualidade de software não é uma característica única. Ela é composta por vários atributos que podem ser avaliados separadamente. Um sistema pode ser funcionalmente correto, mas difícil de usar. Pode ser rápido, mas inseguro. Pode ser bonito, mas impossível de manter.

Por isso, analisar qualidade exige observar diferentes dimensões. Cada dimensão responde a uma pergunta: o sistema faz o que deve? É seguro? É confiável? É fácil de usar? É fácil de modificar? Usa recursos de forma eficiente? Consegue rodar em outros ambientes?

---

## 1. Funcionalidade

### Para que serve

Serve para avaliar se o software cumpre as tarefas que deveria cumprir.

### Explicação detalhada e realista

Funcionalidade está ligada diretamente aos requisitos funcionais. Um sistema de biblioteca deve cadastrar livros, registrar empréstimos, controlar devoluções e emitir relatórios. Se essas funções não existem ou funcionam incorretamente, o sistema falha em funcionalidade.

A funcionalidade também inclui adequabilidade, acurácia, segurança de acesso e interoperabilidade, dependendo do tipo de programa.

### Metáfora

Funcionalidade é o “faz o que promete” do software.

### Situações de uso / exemplo real

Um sistema financeiro que calcula impostos com erro pode ter interface boa, mas falha em acurácia funcional.

### Como posso aplicar no dia a dia

Ao testar um projeto, verifique caso por caso: cada função solicitada existe? Produz resultado correto? Respeita regras?

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]

---

## 2. Segurança

### Para que serve

Serve para proteger funções, dados e acessos contra uso indevido.

### Explicação detalhada e realista

Segurança de acesso envolve garantir que apenas usuários autorizados possam executar determinadas funções. Não basta o sistema “ter login”; é preciso testar concessão e retirada de privilégios, permissões por perfil, acesso a telas, APIs e dados sensíveis.

A segurança é uma característica transversal. Ela não pertence apenas a uma tela; atravessa requisitos, arquitetura, [[09 - Banco de Dados e SGBD - Parte 1|banco de dados]], código e implantação.

### Metáfora

Segurança é como controle de acesso em um prédio. Não basta ter porta na entrada se qualquer pessoa consegue entrar nas salas internas.

### Situações de uso / exemplo real

Um usuário comum não deve acessar tela de administração. Um funcionário desligado deve perder acesso. Um relatório sensível deve exigir permissão adequada.

### Como posso aplicar no dia a dia

Em projetos, separe usuários por perfil. Teste se cada perfil só acessa o que deveria.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[12 - Introdução à Segurança da Informação]]
- [[14 - Roubo de Informações, Identidade e Autenticação Digital]]

---

## 3. Manutenibilidade

### Para que serve

Serve para avaliar se o software pode ser entendido, corrigido, modificado e evoluído com custo aceitável.

### Explicação detalhada e realista

Manutenibilidade é fundamental porque software muda. Um código sem organização, sem nomes claros, sem modularidade, sem testes e sem documentação pode até funcionar hoje, mas se torna caro amanhã.

Subcaracterísticas como analisabilidade, modificabilidade, estabilidade e testabilidade ajudam a avaliar se a manutenção será viável. Um sistema manutenível permite localizar defeitos, entender impactos, alterar sem quebrar tudo e testar mudanças.

### Metáfora

Manutenibilidade é como a organização de uma oficina. Se ferramentas, peças e manuais estão no lugar certo, o conserto é rápido. Se tudo está espalhado, qualquer reparo vira sofrimento.

### Situações de uso / exemplo real

Um sistema com regras de desconto duplicadas em várias partes do código dificulta manutenção. Alterar a regra exige procurar e corrigir múltiplos pontos.

### Como posso aplicar no dia a dia

Evite duplicação, use nomes claros, separe responsabilidades, escreva funções menores e mantenha testes.

### Relações com outras notas

- [[10 - Manutenção de Software e Rastreabilidade]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

---

## 4. Usabilidade

### Para que serve

Serve para avaliar se o software é compreensível, aprendível, operável e agradável para o usuário.

### Explicação detalhada e realista

Usabilidade não é apenas aparência. Um sistema pode ser bonito e ainda ser confuso. Usabilidade envolve permitir que o usuário entenda o fluxo, execute tarefas com poucos erros, receba mensagens claras e consiga aprender o sistema sem esforço exagerado.

Esse atributo está ligado à experiência real de uso. Quando a usabilidade é baixa, aumentam suporte, treinamento, erros operacionais e rejeição do sistema.

### Metáfora

Usabilidade é como sinalização em um aeroporto. Mesmo que o prédio seja moderno, se as placas forem confusas, as pessoas se perdem.

### Situações de uso / exemplo real

Uma tela de venda com muitos campos desorganizados aumenta erros. Uma interface bem agrupada por cliente, produtos, pagamento e entrega reduz confusão.

### Como posso aplicar no dia a dia

Teste suas telas com alguém que não participou do projeto. Observe onde a pessoa hesita ou pergunta o que fazer.

### Relações com outras notas

- [[09 - Prototipação, UX, UI e Validação de Ideias]]

---

## 5. Confiabilidade

### Para que serve

Serve para avaliar se o software mantém funcionamento correto mesmo diante de condições adversas.

### Explicação detalhada e realista

Confiabilidade envolve maturidade, tolerância a falhas e recuperabilidade. Um sistema confiável não apenas funciona em casos ideais; ele lida bem com erros, entradas inesperadas, falhas temporárias e recuperação após problemas.

Confiabilidade é crítica em sistemas financeiros, médicos, industriais e qualquer software que impacte operação real.

### Metáfora

Confiabilidade é como um avião: não basta voar em dia calmo; ele precisa lidar com turbulência, falhas previstas e procedimentos de segurança.

### Situações de uso / exemplo real

Se a internet cai no meio de uma venda, o sistema deve evitar duplicidade, perda de dados ou estado inconsistente.

### Como posso aplicar no dia a dia

Trate erros, valide entradas, registre logs e pense no que acontece quando algo falha.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[12 - Introdução à Segurança da Informação]]
- [[14 - Roubo de Informações, Identidade e Autenticação Digital]]

---

## 6. Eficiência

### Para que serve

Serve para avaliar desempenho e uso adequado de recursos.

### Explicação detalhada e realista

Eficiência envolve tempo de resposta, consumo de memória, uso de CPU, acesso a banco e escalabilidade. Um sistema pode estar funcionalmente correto, mas ser inadequado se demora demais ou consome recursos excessivos.

Eficiência deve ser avaliada conforme contexto. Um relatório mensal pode demorar alguns segundos; uma validação de login não deveria.

### Metáfora

Eficiência é como consumo de combustível. Um carro pode chegar ao destino, mas se gastar demais ou for lento demais, sua operação se torna ruim.

### Situações de uso / exemplo real

Uma consulta sem índice no banco pode funcionar com 100 registros, mas travar com 1 milhão.

### Como posso aplicar no dia a dia

Teste com dados próximos do real. Não avalie desempenho apenas com banco pequeno de teste.

### Relações com outras notas

- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[12 - Introdução à Segurança da Informação]]
- [[14 - Roubo de Informações, Identidade e Autenticação Digital]]

---

## 7. Portabilidade

### Para que serve

Serve para avaliar se o software pode ser adaptado ou executado em diferentes ambientes.

### Explicação detalhada e realista

Portabilidade envolve adaptabilidade, coexistência e substitutibilidade. Um sistema portável é menos preso a uma máquina, sistema operacional, banco ou configuração específica.

Esse atributo é importante quando o software precisa funcionar em Windows e Linux, desktop e mobile, nuvem e servidor local ou diferentes versões de banco de dados.

### Metáfora

Portabilidade é como uma mala bem organizada para viagem. Quanto menos dependências desnecessárias, mais fácil mudar de ambiente.

### Situações de uso / exemplo real

Uma aplicação web que funciona em diferentes navegadores e dispositivos tem maior portabilidade do que uma aplicação dependente de configuração local específica.

### Como posso aplicar no dia a dia

Evite caminhos fixos, configurações espalhadas e dependência de ambiente sem documentação.

### Relações com outras notas

- [[10 - Manutenção de Software e Rastreabilidade]]

## Pontos importantes para prova ou revisão

- Qualidade é multidimensional.
- Funcionalidade verifica se o sistema faz o que deve.
- [[12 - Introdução à Segurança da Informação|Segurança]] controla acesso e proteção.
- [[10 - Manutenção de Software e Rastreabilidade|Manutenibilidade]] determina facilidade de evolução.
- Usabilidade avalia experiência de uso.
- Confiabilidade avalia comportamento sob falhas.
- Eficiência avalia desempenho e recursos.
- Portabilidade avalia adaptação a ambientes diferentes.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Funcionalidade | Capacidade de cumprir tarefas previstas |
| Segurança | Controle de acesso e proteção de dados/funções |
| Manutenibilidade | Facilidade de modificar e corrigir |
| Usabilidade | Facilidade de aprender e operar |
| Confiabilidade | Capacidade de funcionar corretamente ao longo do tempo |
| Eficiência | Relação entre desempenho e uso de recursos |
| Portabilidade | Capacidade de adaptação a diferentes ambientes |

## Possíveis notas futuras

- ISO/IEC 25010
- Métricas de qualidade
- Testabilidade
- [[12 - Introdução à Segurança da Informação|Segurança]] de software
- Usabilidade e heurísticas de Nielsen

## Fonte

Material usado como base:

- Nome do arquivo: 04-parte1-Qualidade de Software.pdf
- Tipo do arquivo: PDF
- Matéria: Engenharia de Software I
