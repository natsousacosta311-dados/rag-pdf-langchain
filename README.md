# 📄 RAG com PDFs — LangChain + LLM

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![LangChain](https://img.shields.io/badge/LangChain-000000?style=for-the-badge&logo=chainlink&logoColor=white)](https://langchain.com)
[![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)
[![FAISS](https://img.shields.io/badge/FAISS-005571?style=for-the-badge)](https://github.com/facebookresearch/faiss)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

> Sistema de perguntas e respostas baseado em documentos PDF, utilizando **RAG** *(Retrieval-Augmented Generation)* para recuperar contexto relevante e gerar respostas precisas com LLM.

---

## 🎯 Objetivo

Criar uma interface inteligente capaz de **responder perguntas sobre o conteúdo de documentos PDF**, combinando busca semântica com geração de linguagem para produzir respostas contextualizadas e fundamentadas.

---

## 🏗️ Arquitetura

```
PDF(s) → Chunking → Embeddings → FAISS (Índice Vetorial)
                                        ↓
Pergunta do usuário → Embedding → Busca por Similaridade
                                        ↓
                    Contexto Recuperado + Pergunta → LLM → Resposta
```

---

## ✨ Funcionalidades

- 📥 **Ingestão de PDFs** — Carregamento e divisão de documentos em chunks otimizados
- 🧠 **Geração de Embeddings** — Representação vetorial semântica do conteúdo
- 🔍 **Busca Semântica** — Recuperação dos trechos mais relevantes via FAISS
- 💬 **Geração de Respostas** — Respostas contextualizadas e fundamentadas no documento

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| **LangChain** | Orquestração do pipeline RAG |
| **OpenAI API** | LLM para geração de respostas e embeddings |
| **FAISS** | Banco vetorial para busca por similaridade |
| **PyPDF / PDFPlumber** | Extração de texto dos PDFs |
| **Python 3.10+** | Linguagem base do projeto |

---

## ⚙️ Pré-requisitos

- Python 3.10 ou superior
- Chave de API da OpenAI

---

## 🚀 Instalação e Uso

### 1. Clone o repositório

```bash
git clone https://github.com/natsousacosta311-dados/rag-pdf-langchain.git
cd rag-pdf-langchain
```

### 2. Crie e ative o ambiente virtual

```bash
python -m venv venv
source venv/bin/activate      # Linux/macOS
venv\Scripts\activate         # Windows
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

### 4. Configure a variável de ambiente

```bash
# Crie um arquivo .env na raiz do projeto
OPENAI_API_KEY=sua-chave-aqui
```

### 5. Execute o sistema

```bash
python main.py
```

---

## 📂 Estrutura do Projeto

```
rag-pdf-langchain/
│
├── data/               # PDFs de entrada
├── embeddings/         # Índice FAISS gerado
├── main.py             # Ponto de entrada da aplicação
├── requirements.txt    # Dependências
├── .env.example        # Exemplo de variáveis de ambiente
└── README.md
```

---

## 📌 Aprendizados e Próximos Passos

- [x] Pipeline RAG funcional com PDFs
- [x] Busca semântica com FAISS
- [ ] Interface web com Streamlit
- [ ] Suporte a múltiplos documentos simultâneos
- [ ] Avaliação de qualidade das respostas (RAGAS)

---

## 👩‍💻 Autora

**Natasha de Sousa Costa** — AI Engineer | Data Scientist

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/seu-perfil)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/natsousacosta311-dados)


Fique à vontade para se conectar ou trocar ideias! 🚀

⭐ Contribuição

Sugestões e melhorias são sempre bem-vindas!
