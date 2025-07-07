# 🗂️ Oracle SQL Scripts – Consultas úteis

[![Oracle](https://img.shields.io/badge/Oracle-DB-F80000?logo=oracle&logoColor=white)](https://www.oracle.com/database/)  
📖 Coleção de **scripts SQL para administração e diagnóstico em bancos Oracle**. Inclui consultas sobre alert logs, ASCII, DB Links, views e outros itens frequentemente utilizados em operações, auditorias e migrações.

---

## 📑 Sumário

- [🔔 consultar_alert_log_11g.sql](#-consultar_alert_log_11gsql)
- [🔡 consultar_ascii.sql](#-consultar_asciisql)
- [🌐 consultar_db_links_em_view_mviews_e_dblinks.sql](#-consultar_db_links_em_view_mviews_e_dblinkssql)
- [📊 consultar_disponibilidade_bds.sql](#-consultar_disponibilidade_bdssql)
- [📈 consultar_hwm_db.sql](#-consultar_hwm_dbsql)
- [🗄️ consultar_tamanho_banco_dados.sql](#-consultar_tamanho_banco_dadossql)
- [🔑 listar_passwordfile_users.sql](#-listar_passwordfile_userssql)
- [👀 listar_todas_visoes_dinamicas.sql](#-listar_todas_visoes_dinamicassql)

---

## 🔔 consultar_alert_log_11g.sql
Consulta a tabela `X$DBGALERTEXT`, uma **view dinâmica do Oracle** que expõe o conteúdo do **alert log** diretamente no banco de dados.  

---

## 🔡 consultar_ascii.sql
Gera uma tabela com os **caracteres ASCII estendidos (33 a 255)**:  
- Mostra o código numérico e símbolo correspondente.  
- Organiza a saída em colunas, com **8 caracteres por linha**.  

---

## 🌐 consultar_db_links_em_view_mviews_e_dblinks.sql
📋 Inventário completo de todos os objetos que **usam ou são database links** no banco.  

**Utilidade:**  
- 🔍 Auditar dependências externas (quem acessa outros bancos).  
- 📦 Planejar migrações (identificar o que depende de DB Links).  
- 🚨 Evitar quebras caso um DB Link seja removido ou alterado.  

---

## 📊 consultar_disponibilidade_bds.sql
Gera um **relatório mensal de disponibilidade** dos bancos monitorados pelo OEM:  
- ⏱ **Total monitorado** (dias).  
- ❌ **Tempo indisponível** (dias).  
- ✅ **Percentual de disponibilidade**, agrupado por banco e mês.  

---

## 📈 consultar_hwm_db.sql
Consulta os **limites já alcançados** de objetos e outros itens no banco, como:  
- Sessões ativas.  
- Total de sessões.  
- E outros recursos monitoráveis.  

---

## 🗄️ consultar_tamanho_banco_dados.sql
Verifica o **tamanho total físico do banco**, considerando:  
- Datafiles.  
- Tempfiles.  
- Redo Logs.  

---

## 🔑 listar_passwordfile_users.sql
Lista os usuários com privilégios administrativos, como:  
- `SYSDBA`.  
- `SYSOPER`.  
- Outros privilégios críticos.  

---

## 👀 listar_todas_visoes_dinamicas.sql
Exibe os **nomes e descrições** de todas as **views e tabelas do sistema** que podem ser consultadas para obter informações sobre o banco.  

---

## 🚀 Como usar
📂 Execute os scripts diretamente no **SQL*Plus**, SQLcl, SQL Developer ou qualquer outra ferramenta compatível com Oracle.  

---

## 🛠️ Requisitos
- Oracle Database 11g ou superior.
- Acesso com privilégios para consultar as views de sistema.  

---
