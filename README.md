📊 RAG com PDFs usando LangChain

Este projeto implementa uma solução de Recuperação Aumentada Generativa (RAG) para consulta inteligente em documentos PDF, utilizando modelos de linguagem (LLMs) e busca semântica.

O objetivo é permitir que perguntas sejam respondidas com base no conteúdo de documentos, retornando respostas contextualizadas e mais precisas.

🚀 Tecnologias utilizadas
Python
LangChain
OpenAI
FAISS
PyPDFLoader
🧠 Como funciona

O projeto segue a arquitetura de RAG:

Leitura de documentos PDF
Divisão do texto em chunks com sobreposição
Geração de embeddings vetoriais
Armazenamento em banco vetorial
Recuperação dos trechos mais relevantes
Geração de resposta com LLM baseada no contexto
⚙️ Estrutura do projeto
.
├── documentos/        # PDFs utilizados como base de conhecimento
├── memrag.py          # Script principal
├── .env               # Chave da API
└── README.md
🔧 Como executar
1. Clone o repositório
git clone https://github.com/seu-usuario/rag-pdf-langchain.git
cd rag-pdf-langchain
2. Crie o arquivo .env
OPENAI_API_KEY=sua_chave_aqui
3. Instale as dependências
pip install -r requirements.txt
4. Execute o projeto
python main_rag.py
💬 Exemplo de uso
responder("Como proceder em caso de roubo com cartão platinum?")

O sistema irá:

Buscar os trechos mais relevantes nos PDFs
Gerar uma resposta baseada no contexto
📈 Melhorias futuras
Integração com Apache Airflow para orquestração de pipelines
Deploy como API (FastAPI ou Flask)
Integração com banco de dados vetorial em nuvem
Interface web para interação com o usuário
Implementação de técnicas de reranking
📌 Observações

Este projeto foi desenvolvido como parte dos meus estudos em Engenharia de IA, com foco em aplicações práticas de LLMs e sistemas de recuperação de informação.

🤝 Contato

Fique à vontade para se conectar ou trocar ideias! 🚀

⭐ Contribuição

Sugestões e melhorias são sempre bem-vindas!
