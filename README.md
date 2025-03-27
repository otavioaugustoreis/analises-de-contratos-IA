# 🧠 Legal Insight Engine - Análise de Contratos com IA

<div align="center">
  <img src="https://img.shields.io/badge/Licença-MIT-blue" alt="Licença MIT">
  <img src="https://img.shields.io/badge/Python-3.10%2B-yellow" alt="Python 3.10+">
  <img src="https://img.shields.io/badge/.NET-8.0-purple" alt=".NET 8">
  <img src="https://img.shields.io/badge/LangChain-0.1%2B-orange" alt="LangChain">
</div>

Solução avançada que integra **LangChain (Python)** com **.NET 8 (C#)** para análise automatizada de documentos jurídicos utilizando IA.

## ✨ Funcionalidades Principais

| Ícone | Funcionalidade | Descrição |
|-------|---------------|-----------|
| 🔍 | Análise de Cláusulas | Identificação automática de termos e cláusulas críticas |
| 📊 | Score de Risco | Classificação de 0-10 com justificativas detalhadas |
| 📑 | Multi-formatos | Suporte a PDF, DOCX e texto puro |
| ⚖️ | Jurisprudência | Comparação com base legal e contratos similares |
| 🔒 | Integração Segura | Comunicação criptografada entre serviços C# e Python |

## 🛠 Stack Tecnológica

```mermaid
graph TD
  A[Frontend] --> B[API .NET]
  B --> C[Serviço Python]
  C --> D[(ChromaDB)]
  C --> E[(Redis)]
  B --> F[(SQL Server)]
