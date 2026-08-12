---
materia: Engenharia de Software I
aula: 14
tags:
  - engenharia-de-software
  - métricas
  - estimativas
  - pontos-de-funcao
  - loc
  - viabilidade
---

## Introdução

Durante o desenvolvimento de software, uma das maiores dificuldades é prever quanto tempo, dinheiro e esforço serão necessários para concluir um projeto. Para reduzir essa incerteza, a Engenharia de Software utiliza métricas e técnicas de estimativa que auxiliam no planejamento, controle de custos e tomada de decisões.

Além das estimativas, é necessário avaliar se o projeto realmente vale a pena ser desenvolvido. Essa avaliação ocorre por meio da análise de viabilidade, responsável por verificar aspectos técnicos, econômicos, operacionais e organizacionais antes do início do projeto. 

## Palavras-chave

Métrica, Estimativa, Custo, Esforço, LOC, SLOC, Pontos de Função, FP, Produtividade, Viabilidade, Cronograma, Stakeholder.

---

# Métricas de Software

## Para que servem

As métricas permitem medir características de um software ou processo de desenvolvimento.

Elas auxiliam na:

- Estimativa de prazo;
- Estimativa de custo;
- Medição de produtividade;
- Comparação entre projetos;
- Planejamento de recursos;
- Avaliação de desempenho da equipe.

Sem métricas, o gerenciamento de projetos depende apenas de percepção e experiência pessoal.

## Explicação técnica

Uma métrica é uma medida utilizada para quantificar algum aspecto do software.

Exemplos:

- Quantidade de linhas de código;
- Quantidade de funcionalidades;
- Tempo gasto no desenvolvimento;
- Número de defeitos encontrados;
- Produtividade da equipe.

Essas informações servem como base para futuras estimativas e tomadas de decisão.

## Situação de uso

Uma empresa deseja desenvolver um novo sistema.

Antes de iniciar o projeto, ela precisa responder perguntas como:

- Quanto custará?
- Quantas pessoas serão necessárias?
- Quanto tempo levará?

As métricas fornecem dados para responder essas questões.

## Aplicação no dia a dia

Mesmo em projetos acadêmicos é possível utilizar métricas para:

- Estimar tempo de estudo;
- Planejar trabalhos;
- Medir produtividade;
- Avaliar evolução de projetos pessoais.

---

# Estimativas de Software

## Para que servem

Estimativas são utilizadas para prever:

- Esforço necessário;
- Prazo de desenvolvimento;
- Quantidade de profissionais;
- Custos do projeto.

Elas ajudam a organização a decidir se um projeto é viável e quanto investimento será necessário. 

## Explicação técnica

Segundo o material, existem duas abordagens principais para estimativas. 

### Técnicas Baseadas em Experiência

Utilizam o conhecimento adquirido em projetos anteriores.

O gerente analisa:

- Projetos semelhantes;
- Complexidade do sistema;
- Experiência da equipe;
- Histórico da organização.

A estimativa é construída a partir de julgamentos fundamentados. 

### Modelagem Algorítmica de Custos

Utiliza modelos matemáticos para calcular esforço e custo.

São considerados fatores como:

- Tamanho do software;
- Complexidade;
- Processo de desenvolvimento;
- Experiência da equipe. 

## Incerteza nas estimativas

Uma característica importante é que estimativas nunca são exatas.

Projetos de software envolvem:

- Mudanças de requisitos;
- Problemas técnicos;
- Diferenças de produtividade;
- Fatores humanos.

Por isso toda estimativa possui um grau de incerteza.

## Metáfora

Fazer uma estimativa de software é semelhante a estimar o tempo de uma viagem longa.

Mesmo conhecendo a rota, fatores como trânsito, clima e imprevistos podem alterar significativamente o resultado.

---

# Estimativas Baseadas em Linhas de Código (LOC)

## Para que serve

A técnica LOC (Lines of Code) mede o tamanho de um software com base na quantidade de linhas de código produzidas. 

## Explicação técnica

É uma das formas mais simples de medição.

A ideia é que sistemas maiores tendem a exigir mais esforço de desenvolvimento.

### LOC

Conta todas as linhas existentes no código.

Problema:

- Não diferencia comentários;
- Não diferencia linhas vazias;
- Não considera complexidade. 

### SLOC

Para aumentar a precisão surgiu o SLOC (Source Lines of Code).

Nesse método:

- Comentários são ignorados;
- Linhas em branco não são consideradas. 

## Limitações

A principal limitação é que quantidade não significa complexidade.

Dois programas podem possuir:

- Mesmo número de linhas;
- Complexidades completamente diferentes.

Por isso LOC é considerada uma métrica simples, porém imprecisa. 

## Situação real

Um sistema de cadastro pode possuir 5.000 linhas de código.

Outro sistema com integração bancária pode possuir as mesmas 5.000 linhas.

Apesar do mesmo tamanho, a complexidade é muito diferente.

---

# Pontos de Função (FP)

## Para que serve

A Análise por Pontos de Função busca medir o tamanho funcional do software sob a perspectiva do usuário. 

É uma das métricas mais importantes da Engenharia de Software.

## Explicação técnica

Diferentemente do LOC, os Pontos de Função não analisam o código.

Eles analisam:

- O que o sistema faz;
- Quais funcionalidades oferece;
- Quais dados manipula.

Isso permite medir o sistema antes mesmo da implementação. 
## Componentes avaliados

A contagem considera cinco elementos principais. 
### Arquivos Lógicos Internos (ALI)

Dados mantidos pelo próprio sistema.

Exemplos:

- Clientes;
- Funcionários;
- Produtos. 

### Arquivos de Interface Externa (AIE)

Dados mantidos por sistemas externos.

Exemplo:

- Tabela oficial de cidades;
- Dados vindos de outro sistema. 

### Entradas Externas (EE)

Informações inseridas no sistema.

Exemplos:

- Cadastro de cliente;
- Cadastro de funcionário. 
### Saídas Externas (SE)

Informações enviadas para fora do sistema.

Exemplos:

- Relatórios;
- Arquivos exportados.

### Consultas Externas (CE)

Informações consultadas sem alterar dados.

Exemplos:

- Login;
- Consultas;
- Pesquisas.
## Fatores de Ajuste

Após a contagem dos Pontos de Função, é necessário considerar características que influenciam a complexidade do sistema. 

Entre elas:

- Comunicação de dados;
- Desempenho;
- Reusabilidade;
- Interface com usuário;
- Processamento complexo;
- Flexibilidade para mudanças;
- Volume de transações. 

Cada característica recebe um peso de influência.

O resultado gera os Pontos de Função Ajustados (PFA). 

## Por que Pontos de Função são importantes?

Porque medem valor funcional entregue ao usuário.

Enquanto LOC mede quantidade de código, FP mede funcionalidades.

Por esse motivo é uma métrica muito mais utilizada em estimativas profissionais.

## Metáfora

LOC mede quantos tijolos foram usados para construir uma casa.

Pontos de Função medem quantos cômodos úteis a casa possui.

Do ponto de vista do usuário, a segunda informação costuma ser mais importante.

## Situação real

Uma empresa recebe um projeto contendo:

- Cadastro de usuários;
- Cadastro de departamentos;
- Controle de permissões;
- Relatórios.

Essas funcionalidades podem ser convertidas em Pontos de Função para estimar:

- Prazo;
- Equipe necessária;
- Custo do projeto. 
---

# Produtividade e Estimativa de Custos

## Para que serve

Após calcular os Pontos de Função, é possível estimar prazo e custo.

## Explicação técnica

A organização utiliza históricos anteriores para definir produtividade.

Exemplo:

Equipe produz:

- 10 FP por dia.

Projeto estimado:

- 46 FP.

Prazo:

46 ÷ 10 = aproximadamente 5 dias.

Se cada FP custar R$100:

46 × 100 = R$4.600,00.

## Aplicação prática

Empresas utilizam esse modelo para:

- Elaborar propostas;
- Definir contratos;
- Planejar equipes;
- Negociar valores com clientes.

---

# Análise de Viabilidade

## Para que serve

A análise de viabilidade determina se vale a pena desenvolver o sistema proposto.
Ela auxilia stakeholders na tomada de decisão sobre continuar ou não um projeto.

## Explicação técnica

A análise de viabilidade ocorre após a definição dos requisitos de negócio e antes do desenvolvimento efetivo do sistema. 

Seu objetivo é responder perguntas como:

- O projeto é tecnicamente possível?
- O custo compensa os benefícios?
- Existe prazo suficiente?
- A organização está preparada para utilizar a solução?

## Tipos de viabilidade

### Viabilidade Organizacional

Avalia alinhamento com objetivos estratégicos da organização. 

### Viabilidade Operacional

Verifica se a solução atende às necessidades do negócio e dos usuários. 

### Viabilidade Econômica

Analisa custo versus benefício. 

### Viabilidade Técnica

Avalia tecnologia, equipe, infraestrutura e conhecimento necessário. 

### Viabilidade de Cronograma

Verifica se o prazo disponível é compatível com o esforço estimado. 

## Metáfora

Antes de construir uma casa, é necessário verificar:

- Terreno;
- Recursos financeiros;
- Tempo disponível;
- Materiais;
- Equipe.

A análise de viabilidade faz exatamente isso para projetos de software.

## Situação real

Uma empresa deseja desenvolver um sistema com Inteligência Artificial.

A análise de viabilidade pode concluir que:

- A tecnologia é adequada;
- Existe retorno financeiro esperado;
- Porém a equipe não possui conhecimento suficiente.

Nesse caso pode ser necessário treinamento ou contratação antes do início do projeto.

## Aplicação no dia a dia

A análise de viabilidade também pode ser aplicada em:

- Escolha de cursos;
- Projetos pessoais;
- Investimentos;
- Empreendimentos;
- Planejamento de carreira.

## Relações com outras notas

- [[11 - Planejamento e Gerenciamento de Projetos em Software]]
- [[07 - Requisitos de Software e Engenharia de Requisitos]]
- [[08 - Gerência de Requisitos, Controle de Mudanças e Configuração]]
- [[05 - Qualidade de Software, Inspeções e Custo da Qualidade]]
- [[10 - Manutenção de Software e Rastreabilidade]]

## Resumo Final

Métricas e estimativas são fundamentais para planejar projetos de software. As estimativas podem ser baseadas em experiência ou em modelos matemáticos. Entre as métricas mais utilizadas estão LOC e Pontos de Função, sendo esta última mais precisa por medir funcionalidades do ponto de vista do usuário. Após as estimativas, realiza-se a análise de viabilidade, responsável por verificar se o projeto é técnica, econômica, operacional, organizacional e temporalmente viável. Essas práticas permitem reduzir riscos, melhorar o planejamento e aumentar as chances de sucesso do projeto.