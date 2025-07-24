# Modelagem de Dados - Artigo Alura

## O que são

Modelos lógicos e físicos que descrevem como os dados estão relacionados. Servem como base sólida para a construção de sistemas eficazes, garantindo integridade, consistência e qualidade dos dados.

## Aplicações da Modelagem de Dados

**Comércio eletrônico e empresas**  
Usada para compreender o comportamento do cliente, prever futuras demandas e personalizar recomendações.

**Saúde e ciências**  
No gerenciamento de registros médicos, permite análise de resultados, previsão de surtos e desenvolvimento de tratamentos.

**Finanças e serviços**  
Na detecção de fraudes, análise de risco de crédito, previsão de tendências e otimização de processos. Bancos usam para avaliar saúde financeira dos clientes, identificar transações e oferecer produtos personalizados.

**Manufatura e logística**  
Ajuda na otimização de processos, gerenciamento de inventários, previsão de demanda e planejamento de rotas. Também permite monitorar o desempenho de máquinas, identificar gargalos e melhorar a eficiência operacional.

**Educação e pesquisa**  
Permite análise de desempenho, previsão de tendências, descoberta de novos conhecimentos e acompanhamento do progresso dos alunos.

## Objetivos da Modelagem de Dados

**Precisão de dados**  
Garante dados armazenados livres de erros, com definição clara de tipos, formatos e restrições.

**Integridade de dados**  
Assegura que os dados sejam consistentes em todo o sistema.

**Consistência de dados**  
Garante interpretação uniforme por todas as partes do sistema, através de convenções padronizadas na organização.

## Tipos de Modelagem

### Conceitual

Representação abstrata, independente do sistema. Usa elementos como entidades, atributos e seus relacionamentos. Captura os requisitos dos usuários finais. Representada por diagramas como:

- Diagrama de Entidade-Relacionamento (DER)
- Modelagem de objetos



### Lógica

Traduz a modelagem conceitual com mais detalhes. Define chaves primárias, estrangeiras e outras restrições. Ainda é abstrata, mas próxima da implementação. Representada por:

- Modelo de dados relacional



### Física

Estágio final: implementada num SGBD específico. Define tipos de dados, índices, particionamentos, etc. Otimizada para a plataforma usada. Representada por:

- Scripts de criação de banco de dados



## Desafios e Considerações

A complexidade dos sistemas exige compreensão profunda dos requisitos. Mudanças nas necessidades do negócio exigem modelos adaptáveis. Versões diferentes precisam manter a consistência. A escalabilidade é essencial para evitar problemas de desempenho e manutenção.

## Boas Práticas na Modelagem

- Envolver partes interessadas  
- Utilizar metodologias de modelagem  
- Priorizar a flexibilidade  
- Adotar boas práticas de design  
- Manter documentação atualizada  

## Benefícios

- Melhor tomada de decisão com dados precisos  
- Maior eficiência interna  
- Melhoria na qualidade dos dados  
- Redução de custos operacionais  
- Maior competitividade  
- Melhor satisfação do cliente  
- Suporte a iniciativas estratégicas  
- Maximiza o uso de dados no longo prazo  

---

# MER & DER - Artigo Alura

## O que é MER (Modelo Entidade-Relacionamento)

Descreve objetos do mundo real por meio de entidades, seus atributos e relacionamentos.

### Entidades

Objetos com existência independente (ex: pessoas, carros). Podem ser:

- Fortes: independem de outras entidades  
- Fracas: dependem de entidades fortes  
- Associativas: ligam uma entidade a um relacionamento  

### Atributos

Propriedades das entidades:

- Simples: indivisíveis (CPF)  
- Compostos: divisíveis (endereço → rua, cidade)  
- Multivalorados: vários valores (telefones)  
- Derivados: dependem de outros atributos (idade a partir de data de nascimento)  
- Chave: valor único que identifica a entidade (CPF)  

### Relacionamentos

Conexões entre entidades, expressas com verbos. Tipos:

- 1:1 — um para um  
- 1:N — um para muitos  
- N:N — muitos para muitos  

## DER (Diagrama Entidade-Relacionamento)

Representação gráfica do MER.

### Exemplo Prático

Instituição precisa de sistema para controle de custos, com informações de alunos, cursos e professores. Entidades:

- Alunos: matrícula, nascimento, idade  
- Cursos: descrição, quantidade de alunos  
- Professores: nome  

Relacionamentos: aluno-curso, professor-curso, professor-aluno


---

# Modelagem de Dados - Curso Alura

## Alinhamento de Desenvolvimento

O modelo conceitual deve ser referência comum do time. A modelagem em etapas divide responsabilidades e padroniza informações.

## Etapas da Modelagem

### Mini-mundo

Parte do mundo real que será representada no sistema. Define o escopo e os dados relevantes.

### Levantamento de Requisitos

Feito com o cliente. Define funcionalidades e dados necessários. Baseia-se em perguntas como:

- Quais os objetivos do projeto?  
- Quais dados precisam ser armazenados?  
- Quais fontes de dados existem?  

Usa conceitos como abstração para focar no essencial.

### Modelo Conceitual

Primeiro diagrama. Inclui regras de negócio, estrutura dos dados e suas relações. Representado com DER.

### Diagrama de Dados

Ferramenta sugerida: Visual Paradigm. Inclui:

- Entidades (fortes, fracas)  
- Cardinalidade: 1:1, 1:N, N:N  
- Entidades associativas: para transformar N:N em 1:N usando tabelas intermediárias  
