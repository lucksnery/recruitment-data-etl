# Projeto 1 — Pipeline ETL Simples (Python + SQL + Streamlit)

## 📌 Descrição Geral
Este projeto tem como objetivo a construção de um **pipeline ETL (Extract, Transform, Load)** simples, simulando um **cenário real de recrutamento**, onde dados de candidatos são coletados por meio de **formulários web** e frequentemente apresentam **inconsistências, falta de padronização e erros de preenchimento**.

O pipeline realiza a **extração dos dados brutos**, o **tratamento e padronização**, o **armazenamento em banco de dados relacional** e, por fim, a **visualização das informações em um dashboard interativo** desenvolvido com Streamlit.

---

## 🛠️ Tecnologias Utilizadas
- **Python**
- **Pandas**
- **SQLite**
- **Streamlit**
- **CSV (dados brutos)**

---

## 1️⃣ Geração do Arquivo CSV (Dados Brutos)
Nesta etapa, é criado um arquivo **CSV** que simula dados coletados a partir de um **formulário online utilizado por recrutadores**.

Os dados são preenchidos por candidatos e **não seguem um padrão consistente**, apresentando problemas comuns do mundo real, como:
- Datas de nascimento em diferentes formatos  
- Pretensão salarial preenchida como texto, números ou valores incompletos  
- Informações de localização inconsistentes (cidade, estado, abreviações, erros de digitação)  
- Campos vazios ou inválidos  

O objetivo desta etapa é **simular um cenário realista de dados desestruturados**, semelhante ao encontrado em ambientes corporativos.

---

## 2️⃣ Extração e Tratamento dos Dados (Python + Pandas)
Os dados do arquivo CSV são carregados utilizando **Python com a biblioteca Pandas**, sendo transformados em um **DataFrame** para facilitar o processamento.

Nesta fase, são realizadas operações de **limpeza e padronização**, como:
- Normalização de formatos de data  
- Conversão de campos numéricos (ex: pretensão salarial)  
- Tratamento de valores nulos ou inválidos  
- Padronização de textos (ex: cidade, estado, cargo)  
- Validação básica dos dados  

Essa etapa corresponde à fase **Transform** do pipeline ETL.

---

## 3️⃣ Carga dos Dados no Banco de Dados (SQLite)
Após o tratamento, os dados são carregados em um banco de dados **SQLite**, estruturando as informações em tabelas organizadas.

Nesta etapa:
- O banco de dados é criado automaticamente (caso não exista)  
- Os dados tratados são inseridos de forma estruturada  
- O banco passa a servir como **fonte confiável para análises futuras**  

Essa fase representa a etapa **Load** do processo ETL.

---

## 4️⃣ Visualização e Dashboard com Streamlit
Por fim, é desenvolvido um **dashboard interativo utilizando Streamlit**, que consome os dados armazenados no SQLite.

O dashboard apresenta:
- Indicadores gerais (quantidade de candidatos, média salarial, etc.)  
- Gráficos interativos (distribuição por localização, faixa salarial, idade, etc.)  
- Tabelas dinâmicas para consulta dos dados  
- Filtros interativos para análise exploratória  

O objetivo desta etapa é **transformar dados brutos em informações visuais claras e acessíveis**, facilitando a tomada de decisão por recrutadores ou analistas.

---

## 🎯 Objetivo do Projeto
Demonstrar, de forma prática, conhecimentos em:
- Construção de pipelines ETL  
- Manipulação e tratamento de dados com Pandas  
- Armazenamento em banco de dados relacional (SQLite)  
- Criação de dashboards interativos com Streamlit  
- Simulação de problemas reais encontrados em dados do mercado  

---
