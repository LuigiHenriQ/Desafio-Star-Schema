# 🎓 Star Schema - Análise de Professores

Este projeto tem como objetivo transformar um modelo relacional em um **modelo dimensional do tipo estrela (Star Schema)** para análises de dados com foco em professores, cursos ministrados e departamentos.

## 📌 Objetivo

Criar um modelo dimensional otimizado para BI, onde a **fato** central representa os dados de professores, cursos, disciplinas e departamentos, permitindo análises como:

- Quantidade de cursos ministrados por professor
- Relação entre professores e departamentos
- Histórico de disciplinas oferecidas
- Distribuição temporal de cursos/disciplina

## 🛠 Arquivos

- `Desafio_StarSchema.mwb`: Modelo dimensional desenvolvido no MySQL Workbench.
- `documento_base.docx`: Descrição do desafio e orientações.

## 🧱 Modelagem

### ⭐ Tabela Fato

A tabela fato foi construída com foco no **professor como entidade central**, agregando as seguintes medidas e chaves:

- ID do professor
- ID do curso
- ID do departamento
- ID da disciplina
- ID da data (dimensão tempo)
- Carga horária, quantidade de disciplinas, etc.

### 🔷 Tabelas Dimensão

As seguintes dimensões foram criadas:

- `dim_professor`: dados do professor (nome, titulação, etc.)
- `dim_curso`: informações do curso ministrado
- `dim_departamento`: departamento vinculado ao professor
- `dim_disciplina`: disciplinas ministradas
- `dim_tempo`: dimensão de tempo criada artificialmente com campos como:
  - Data
  - Ano
  - Semestre
  - Mês
  - Dia da semana

## 📊 Aplicação

O modelo gerado pode ser utilizado em ferramentas como Power BI, Tableau ou similares para construção de dashboards analíticos voltados à gestão acadêmica e análise de desempenho e oferta educacional por professor.

## ✅ Conclusão

O modelo em estrela facilita análises agregadas e é ideal para ambientes de Data Warehouse. Este exercício simula um cenário real de modelagem dimensional, sendo uma ótima adição ao portfólio de projetos de dados.

---

🧑‍💻 Desenvolvido como parte de desafio acadêmico de modelagem dimensional.
