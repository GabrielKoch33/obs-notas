---
materia: Engenharia de Software I
tipo: aula
status: refeito_por_ia
fonte:
  - 09-parte1-Prototipação.pdf
data_resumo: 2026-05-11
tags:
  - faculdade
  - engenharia-de-software
  - prototipacao
  - ux
  - ui
---

# Prototipação, UX, UI e Validação de Ideias

Esta nota explica prototipação como técnica para visualizar, comunicar e validar requisitos antes ou durante o desenvolvimento. Também diferencia UX e UI, dois conceitos frequentemente confundidos.

## Palavras-chave

- Prototipação
- Protótipo descartável
- Protótipo evolucionário
- UX
- UI
- Interface
- Experiência do usuário
- Validação
- Feedback
- Draw.io

## Resumo geral da aula

Prototipação é útil quando se deseja mostrar aos usuários como poderá ser o resultado final do software ou parte dele. Ela reduz ambiguidades, melhora comunicação e ajuda a validar requisitos.

UX está relacionada à experiência do usuário ao interagir com o sistema. UI está relacionada à interface visual, aparência, apresentação e interatividade. Uma interface bonita não garante boa experiência se o fluxo for confuso.

---

## 1. Para que serve a prototipação

### Para que serve

Serve para transformar ideias abstratas em algo visual, discutível e validável.

### Explicação detalhada e realista

Durante o levantamento de requisitos, usuários podem ter dificuldade para explicar o que querem. O protótipo ajuda a tornar a conversa concreta. Em vez de discutir apenas frases, a equipe mostra uma tela, fluxo ou interação.

Prototipação também ajuda a descobrir problemas cedo. Se o usuário percebe que uma tela não contempla forma de pagamento, desconto ou local de entrega, essa correção é feita antes da implementação.

### Metáfora

Protótipo é um rascunho visual do sistema. Ele permite apagar, riscar e reorganizar antes de pintar o quadro final.

### Situações de uso / exemplo real

Antes de implementar uma tela de venda, a equipe desenha campos de cliente, produtos, descontos, forma de pagamento e entrega. O usuário avalia se o fluxo representa a operação real.

### Como posso aplicar no dia a dia

Antes de codar uma interface, desenhe no papel ou em ferramenta simples. Valide com alguém. Corrigir desenho é mais barato que refazer código.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[04 - Modelos de Desenvolvimento de Software - Cascata, Incremental, Iterativo, V, Espiral e Prototipação]]

---

## 2. UX e UI

### Para que serve

Servem para separar experiência de uso e interface visual.

### Explicação detalhada e realista

UX, ou experiência do usuário, envolve como a pessoa se sente e se comporta ao usar o sistema. Inclui facilidade, clareza, fluxo, confiança, esforço cognitivo e satisfação.

UI, ou interface do usuário, envolve elementos visuais e interativos: botões, cores, campos, menus, ícones, espaçamento, layout e apresentação.

Um sistema pode ter UI bonita e UX ruim. Por exemplo, uma tela visualmente agradável, mas com fluxo confuso, mensagens vagas e muitos passos desnecessários.

### Metáfora

UI é a aparência de uma porta: cor, maçaneta, material. UX é a experiência de atravessar essa porta: se ela abre fácil, se está no lugar certo e se leva ao ambiente esperado.

### Situações de uso / exemplo real

Um botão “Salvar” bonito mas escondido prejudica UX. Um fluxo de compra com poucos passos, mensagens claras e prevenção de erro melhora UX.

### Como posso aplicar no dia a dia

Ao desenhar telas, pense: o usuário entende o que fazer? O caminho é natural? O sistema previne erro? As mensagens ajudam?

### Relações com outras notas

- [[06 - Atributos e Características de Qualidade de Software]]

---

## 3. Protótipo descartável

### Para que serve

Serve para aprender, demonstrar e validar rapidamente, sem intenção de virar o produto final.

### Explicação detalhada e realista

O protótipo descartável é construído durante a engenharia de requisitos para mostrar o que o analista entendeu. Ele pode ser feito rapidamente, em papel ou ferramenta visual. Seu objetivo é comunicação, não produção.

O risco é o cliente achar que o sistema já está quase pronto. Por isso, deve ficar claro que protótipo descartável não possui necessariamente banco de dados, segurança, regras completas ou arquitetura definitiva.

### Metáfora

É como uma maquete de papelão. Ela ajuda a visualizar, mas não é a construção real.

### Situações de uso / exemplo real

Desenhar a tela de entrada de venda em papel para discutir campos, sequência e regras.

### Como posso aplicar no dia a dia

Use protótipos descartáveis para aprender rápido. Depois, implemente corretamente com arquitetura e validações.

### Relações com outras notas

- [[07 - Requisitos de Software e Engenharia de Requisitos]]

---

## 4. Protótipo evolucionário

### Para que serve

Serve para construir uma versão inicial que evolui até se tornar parte do produto final.

### Explicação detalhada e realista

O protótipo evolucionário contém um subconjunto dos requisitos finais. Diferente do descartável, ele é planejado desde o início para evoluir. Cada versão do protótipo alimenta o próximo incremento.

Esse tipo exige mais cuidado técnico. Como ele pode virar produto, não deve ser construído de qualquer forma. Precisa de arquitetura mínima, padrões, testes e controle.

### Metáfora

É como plantar uma muda que será cuidada até virar árvore. Diferente da maquete, ela fará parte do resultado final.

### Situações de uso / exemplo real

Criar uma primeira versão funcional do cadastro de clientes e depois evoluir com validações, permissões e integração.

### Como posso aplicar no dia a dia

Quando souber que o protótipo pode virar produto, não faça gambiarra extrema. Pense em evolução.

### Relações com outras notas

- [[04 - Modelos de Desenvolvimento de Software - Cascata, Incremental, Iterativo, V, Espiral e Prototipação]]

---

## 5. Áreas tratáveis por protótipos

### Para que serve

Serve para identificar onde a prototipação ajuda mais.

### Explicação detalhada e realista

Protótipos podem ser usados para interfaces, relatórios, gráficos, organização de banco de dados, cálculos complexos, tempo de resposta crítico e tecnologias no limite do conhecimento da equipe.

A prototipação é especialmente útil onde há incerteza. Se a equipe não sabe se uma solução técnica é viável, pode criar um pequeno experimento. Se não sabe se a tela atende o usuário, pode criar uma versão visual.

### Metáfora

Protótipo é uma lanterna em ambiente escuro. Ele não constrói o caminho inteiro, mas mostra onde estão obstáculos.

### Situações de uso / exemplo real

Antes de usar uma API nova, a equipe cria um pequeno programa para testar autenticação, resposta e limites.

### Como posso aplicar no dia a dia

Use protótipos para reduzir dúvida: tela, regra, cálculo, banco, integração ou desempenho.

### Relações com outras notas

- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]

## Pontos importantes para prova ou revisão

- Prototipação ajuda na comunicação e validação de requisitos.
- UX é experiência de uso; UI é interface visual.
- Protótipo descartável é feito para aprender e depois descartar.
- Protótipo evolucionário é planejado para evoluir.
- O cliente pode confundir protótipo com software pronto.
- Protótipos são úteis para interface, relatórios, banco, cálculos, desempenho e tecnologia nova.

## Termos técnicos importantes

| Termo | Explicação |
|---|---|
| Protótipo | Versão inicial usada para validar ideia ou requisito |
| Protótipo descartável | Protótipo feito para aprender e descartar |
| Protótipo evolucionário | Protótipo que evolui para o produto |
| UX | Experiência do usuário |
| UI | Interface do usuário |
| Feedback | Retorno do usuário sobre a solução |
| Validação | Confirmação de que a solução atende à necessidade |

## Possíveis notas futuras

- Figma
- Wireframe
- Prototipação de baixa fidelidade
- Prototipação de alta fidelidade
- Teste de usabilidade

## Fonte

Material usado como base:

- Nome do arquivo: 09-parte1-Prototipação.pdf
- Tipo do arquivo: PDF
- Matéria: Engenharia de Software I
