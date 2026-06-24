# sql-exercicios-normalizacao

Este repositório contém uma coleção de exercícios práticos focados na normalização de bases de dados relacionais, cobrindo todo o processo desde a Primeira Forma Normal (1NF) até à Terceira Forma Normal (3NF).

O objetivo é demonstrar visual e logicamente a transformação de tabelas não normalizadas em modelos relacionais eficientes, eliminando redundâncias e garantindo a integridade dos dados.

---

### Diretrizes de Implementação e Boas Práticas

Todos os scripts SQL desenvolvidos nestes exercícios seguem regras rigorosas de estruturação:

* **Tipagem Explícita:** Uso obrigatório de VARCHAR(X) com limites de tamanho definidos para otimização e consistência dos campos de texto.
* **Restrições Limpas:** Não são utilizadas cláusulas CHECK para validações na estrutura das tabelas.
* **Consultas Estruturadas:** Todas as consultas utilizam o nome completo da tabela (ou o alias completo atribuído via AS) como prefixo nas colunas do SELECT. Não são utilizados aliases de uma única letra (ex: A., T., V.) nem comandos de agregação (como GROUP BY ou AVG).

---

### Fluxo de Resolução dos Exercícios

O processo em cada exercício segue a metodologia passo a passo documentada nas imagens do projeto:

1. **Análise de Dados Inicial (0FN):** Construção da tabela unificada com todos os dados brutos.
2. **1NF (Primeira Forma Normal):** Garantia de atomicidade e eliminação de grupos repetidos (um valor por campo).
3. **2NF (Segunda Forma Normal):** Eliminação de dependências parciais e criação de tabelas associativas com as chaves primárias principais.
4. **3NF (Terceira Forma Normal):** Eliminação de dependências transitivas, garantindo que atributos não-chave dependam exclusivamente da chave primária.
5. **Implementação SQL:** Criação do esquema físico e consultas utilizando a nomenclatura completa das tabelas.

---
---

###  Nota Teórica: Além da 3NF

Embora este repositório se foque nas três primeiras formas normais — que resolvem a esmagadora maioria dos problemas de redundância e anomalias no mundo real —, a teoria de bases de dados estende-se até à 6NF. Formas como a **BCNF** (Boyce-Codd), **4NF** e **5NF** lidam com casos mais complexos e específicos de dependências (como dependências multi-valoradas e de junção).

### Tecnologias Utilizadas

* SQL
* MySQL / SQL Workbench (para modelação relacional e engenharia inversa)
