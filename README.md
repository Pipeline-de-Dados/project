# 📊 Pipeline de Dados: do Zero ao Estrelato

Este projeto foi desenvolvido como parte do Bootcamp de Análise de Dados da SoulCode Academy, com o objetivo de aplicar técnicas avançadas de análise de dados na resolução de desafios reais do mercado. A iniciativa busca demonstrar como a automação e a estruturação de dados podem otimizar processos e gerar insights estratégicos para as empresas.

---

## 📌 Sobre o Projeto

Criado para a DM9, o projeto foca na otimização dos processos do setor de Recursos Humanos, abordando desafios como a fragmentação de dados e a execução de tarefas manuais. Por meio de um pipeline eficiente utilizando Python, BigQuery e Power BI, a solução melhora a confiabilidade das informações, aumenta a escalabilidade e reduz custos operacionais. Os impactos incluem:

✅ **Maior eficiência** e **redução de custos operacionais**  
✅ **Melhoria na confiabilidade e escalabilidade** dos processos  
✅ **Geração de insights estratégicos** para a empresa  

---

## 🏢 Sobre a DM9

A [**DM9**](https://www.dm9.com.br/) é uma renomada agência de publicidade brasileira, fundada em 1975 por **Duda Mendonça**. Reconhecida por sua criatividade, foi a primeira agência do Brasil a conquistar o título de "**Agência do Ano**" no **Cannes Lions**. Criou campanhas icônicas como **Mamíferos da Parmalat**, **Pipoca com Guaraná Antarctica** e o comercial do **tetracampeonato do Brasil em 1994**. Em 1989, foi adquirida por **Nizan Guanaes** e **Guga Valente**, consolidando-se como uma das maiores referências do mercado publicitário.

---

## 🛠 Etapas do Projeto

O desenvolvimento deste projeto envolveu várias etapas para garantir um fluxo de dados eficiente, seguro e visualizável.

### 1️⃣ Planejamento e Definição do Problema
📌 Identificação dos desafios enfrentados pelo setor de RH da DM9   
📌 Criação do Diagrama de Fluxo de Dados (DFD) para planejar a estrutura do projeto   
📌 Levantamento de requisitos e definição dos KPIs  
📌 Escolha das ferramentas e tecnologias

### 2️⃣ Modelagem dos Dados

📌 Criação do Diagrama Entidade-Relacionamento (DER) para organizar a estrutura dos dados   
📌 Definição dos relacionamentos entre as tabelas no BigQuery   
📌 Normalização dos dados para otimizar consultas

### 3️⃣ Construção do Pipeline de Dados

📌 Extração dos dados de diversas fontes (JSONs, planilhas, banco de dados)     
📌 Transformação e limpeza utilizando Python e pandas   
📌 Upload dos dados tratados para o Google Cloud Storage e envio ao BigQuery

### 4️⃣ Análise e Geração de Insights

📌 Execução de consultas no BigQuery para identificar padrões   
📌 Aplicação de estatísticas descritivas e cruzamento de informações relevantes     
📌 Identificação de tendências e possíveis melhorias para o setor de RH

### 5️⃣ Visualização dos Dados
📌 Desenvolvimento do dashboard no Power BI para facilitar a interpretação dos dados    
📌 Criação de gráficos interativos e relatórios para os tomadores de decisão    
📌 Compartilhamento do dashboard para análise e feedback dos stakeholders

### 6️⃣ Documentação e Apresentação Final
📌 Redação da documentação do projeto, incluindo este README    
📌 Criação dos slides da apresentação no Figma  
📌 Validação dos resultados com a equipe e ajustes finais


---

## 🛠 Bibliotecas Utilizadas

O projeto utiliza diversas bibliotecas para **manipulação de dados**, **integração com APIs** e **armazenamento na nuvem**. Abaixo estão as principais bibliotecas e suas funções:

### 📂 Manipulação de Dados
- **`pandas`** – Processamento e análise de dados estruturados.  
- **`unicodedata`** – Normalização e tratamento de caracteres especiais.  
- **`re`** – Manipulação de expressões regulares para limpeza e formatação de dados.  
- **`datetime`** – Manipulação de datas para organização e filtragem de informações.  

### 🌐 Integração com APIs e Requisições HTTP
- **`requests`** – Comunicação com APIs via HTTP.  
- **`json`** – Manipulação de dados em formato JSON.  
- **`io`** – Operações de entrada e saída de arquivos em memória.  
- **`os`** – Interação com o sistema operacional.  

### 🔐 Autenticação e Acesso a Serviços do Google
- **`google.oauth2.service_account.Credentials`** – Autenticação via credenciais de conta de serviço.  
- **`googleapiclient.discovery.build`** – Conexão com APIs do Google (ex: Drive, Sheets).  
- **`googleapiclient.http.MediaIoBaseDownload`** – Download de arquivos via API do Google Drive.  
- **`google.cloud.storage`** – Manipulação de arquivos no Google Cloud Storage.  
- **`google.cloud.bigquery`** – Conexão e interação com o BigQuery.  
- **`google.cloud.exceptions.NotFound`** – Tratamento de exceções ao acessar dados no Google Cloud.  
- **`pandas_gbq.to_gbq`** – Envio de DataFrames para o BigQuery.  

### 🏗 Google Colab
- **`google.colab.files`** – Upload e download de arquivos no ambiente do Colab.  
- **`google.colab.auth`** – Autenticação no Google Colab.  

### 🔧 Bibliotecas Instaladas via `pip`
Além das bibliotecas mencionadas, também foram instaladas dependências externas para integração com APIs do Google e autenticação:

```bash
!pip install PyDrive google-api-python-client google-auth google-auth-oauthlib google-cloud-storage requests pyjwt
```

---

## ☁️ Uso do Google Cloud
O Google Cloud desempenha um papel essencial na infraestrutura deste projeto, garantindo armazenamento escalável, processamento eficiente e análises rápidas. Utilizamos os seguintes serviços:

### 🔹BigQuery
O BigQuery é um data warehouse totalmente gerenciado que permite análises rápidas em grandes volumes de dados. Neste projeto, ele é utilizado para:     
✅ Armazenar dados estruturados     
✅ Executar consultas SQL otimizadas    
✅ Gerar insights em tempo real

### 🔹Google Cloud Storage
O Google Cloud Storage permite o armazenamento seguro de arquivos brutos antes do processamento. Suas vantagens incluem:    
✅ Alta disponibilidade e segurança     
✅ Integração com outras ferramentas do Google Cloud    
✅ Escalabilidade para grandes volumes de dados

### 🔹APIs do Google Cloud
Além do armazenamento e processamento, utilizamos APIs do Google Cloud para:

Autenticação e autorização (Google OAuth e Service Accounts)    
Interação com o Google Drive (importação/exportação de arquivos)    
Integração direta com BigQuery usando pandas_gbq


---

## 📂 Estrutura do Repositório
📁 `apresentacao/` – Slides em PDF explicando o projeto  
📁 `dados/` – Arquivos de entrada utilizados na análise  
📁 `diagramas/` – Slides em PDF explicando o projeto  
📁 `notebooks/` – Jupyter Notebooks com códigos Python  


---

## 🏆 Resultados e Impacto

🚀 **Redução de tempo gasto** com análise manual de dados  
📉 **Minimização de erros humanos** na tomada de decisão  
📊 **Aumento da confiabilidade e escalabilidade** das informações  

> **Este projeto foi desenvolvido como parte do Bootcamp de Análise de Dados promovido pela SoulCode Academy em parceria com a Flora Cosméticos e Meio & Mensagem.**

---

## 👥 Equipe do Projeto

👤 **[Álevy Bruno](https://www.github.com/alevybruno)**  
👤 **[Dionísio Ribeiro](https://www.github.com/dionisio2024)**  
👤 **[Joshua Bertocchi](https://www.github.com/JoshuaBertocchi)**  
👤 **[kleiton Santos](https://www.github.com/kleistsux)**  
👤 **[Lorena Gutierrez](https://www.github.com/lorenavelina)**  
👤 **[Lucas Aguiar](https://www.github.com/Lucas-335)**  
👤 **[Matheus Vaz](https://www.github.com/matheusvazdata)**  
👤 **[Nicolly Rodrigues](https://www.github.com/nicky89ck)**  


---

