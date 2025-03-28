# 🧠 Legal Insight Engine - Backend API

<div align="center">
  <img src="https://img.shields.io/badge/Licença-MIT-blue" alt="Licença MIT">
  <img src="https://img.shields.io/badge/Python-3.10%2B-yellow" alt="Python 3.10+">
  <img src="https://img.shields.io/badge/.NET-8.0-purple" alt=".NET 8">
  <img src="https://img.shields.io/badge/LangChain-0.1%2B-orange" alt="LangChain">
  <img src="https://img.shields.io/badge/Backend-Only-green" alt="Backend Only">
</div>

## 📌 Visão Geral
Solução backend para análise automatizada de contratos jurídicos utilizando IA, com integração entre:
- **API .NET 8 (C#)** como camada principal
- **Serviço Python (LangChain)** para processamento de documentos
- **Banco de dados vetorial** para armazenamento de embeddings

## ✨ Funcionalidades Principais
| Ícone | Funcionalidade               | Descrição                                  |
|-------|-----------------------------|--------------------------------------------|
| 🔍    | Extração de Cláusulas       | Identificação automática de termos críticos|
| ⚖️    | Análise de Conformidade     | Verificação com base legal aplicável       |
| 📊    | Score de Risco              | Classificação 0-10 com justificativas      |
| 🔗    | Referência Cruzada          | Ligações entre cláusulas relacionadas      |

## 🛠 Stack Tecnológica
```mermaid
graph TD
  A[API .NET] -->|gRPC/HTTP| B[Serviço Python]
  B --> C[(ChromaDB)]
  B --> D[(Redis)]
  A --> E[(SQL Server)]
````
## 📦 Componentes Principais

### **Camada .NET (C#)**
- ✅ **Endpoints REST** para upload e consulta  
- ✅ **Gerenciamento de usuários** e permissões  
- ✅ **Cache de resultados** para performance  

### **Serviço Python**  
- 🐍 **Processamento de documentos** (PDF, DOCX)  
- 🔢 **Geração de embeddings** com LangChain  
- 🔍 **RAG** (Retrieval-Augmented Generation)  
- 🤖 **Integração com LLMs** (OpenAI/GPT)  

### **Armazenamento**  
- 🗄️ **ChromaDB/FAISS** para vetores  
- ⚡ **Redis** para cache  
- 🗃️ **SQL Server** para metadados  

---

## 🔐 Segurança  
- 🔒 **Comunicação criptografada** entre serviços  
- 👥 **Controle de acesso** baseado em roles  
- 📝 **Logging** de todas as operações  

---

## 🚀 Como Executar  
```bash
# Serviço Python
pip install -r requirements.txt
python service/main.py

# API .NET
dotnet run --project LegalInsight.API

