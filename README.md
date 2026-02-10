# 🎬 Projeto de Banco de Dados – Cinema
**Disciplina:** Gerenciamento de Banco de Dados

Este repositório contém o projeto conceitual, lógico e relacional de um sistema de gerenciamento de cinemas. O trabalho inclui modelagem completa das entidades, relacionamentos e restrições necessárias para representar o domínio.

---

## 📌 Conteúdo do Projeto

### **1. Modelo Entidade-Relacionamento (MER)**
- Entidades: Cinema, Sala, Funcionário, Zelador, Fiscal, Filme, Sessão, Equipamento, Gratificação.
- Relacionamentos: Trabalha, Fiscaliza, Limpa, Exibe, Apresenta.
- Inclui cardinalidades, especializações e atributos derivados.

### **2. Modelo Relacional**
Tradução completa do MER para o modelo relacional, incluindo:
- Chaves primárias (PK) e estrangeiras (FK)
- Tabelas de relacionamentos N:N
- Chaves artificiais quando necessário (ex.: `ID_ARTIFICIAL` em SESSAO)
- Resolução de especializações por herança de chave

---

## 📂 Principais Tabelas
- `CINEMA(CNPJ, END_CEP, END_RUA, END_NUM)`
- `FUNCIONARIO(CPF, SALARIO)`
- `ZELADOR(CPF)`
- `FISCAL(CPF)`
- `SALA(CNPJ, NUMERO, CPF_FISCAL)`
- `FILME(CODIGO, TITULO, CODIGO_FILME_ANTERIOR)`
- `SESSAO(ID_ARTIFICIAL, DATA, HORARIO, CODIGO, CNPJ, NUMERO)`
- `EQUIPAMENTO(ID)`
- `GRATIFICACAO(ID)`
- `LIMPA(CPF, ID, CNPJ, NUMERO, DATA)`
- `TRABALHA(CPF, CNPJ, ID)`

---

## 🛠️ Tecnologias e Técnicas
- Modelagem ER
- Conversão para Modelo Relacional
- Normalização de dados
- Preparação para implementação em SQL

---

## 🎯 Objetivo
Fornecer uma modelagem completa e bem estruturada para apoiar o desenvolvimento de um banco de dados de cinema.

---
