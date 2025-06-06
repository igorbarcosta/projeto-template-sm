# 📄 Relatório de Acompanhamento de Projeto — Sistemas Multiagente

> Preencha com atenção. Este relatório tem o objetivo de **organizar o pensamento, identificar bloqueios e alinhar os próximos passos do seu projeto**.

---

## 🧠 1. Visão Geral do Projeto

- **Título do Projeto**:  
  Agente RAG para Análise de Documentos Jurídicos

- **Integrantes da Equipe**:  
  - Marcos (arquitetura e integração)
  - Sofia (parsing e chunking)
  - Letícia (LLM e interface)

- **Resumo em uma frase**:  
  Um agente que responde perguntas jurídicas a partir de documentos legais internos usando RAG.

---

## ⚙️ 2. Arquitetura Atual

- **Quantos agentes existem no sistema atualmente?**  
  Apenas 1 agente: `AgenteConsultorLegal`.

- **Função principal de cada agente:**  
  Receber perguntas e buscar trechos relevantes em uma base vetorial para gerar uma resposta fundamentada.

- **Eles interagem entre si? Como?**  
  Ainda não. A ideia futura é criar um agente de parsing separado e outro de curadoria de resposta.

- **Já existe algum ambiente de simulação/teste?**  
  Sim. Interface básica no Gradio para simular perguntas e ver a resposta do sistema.

---

## ✅ 3. Avanços Concretos

- Parser funcional para documentos `.docx` (com alguma limitação em tabelas).
- Chunking básico com `RecursiveCharacterTextSplitter` da LangChain.
- Criação inicial da base vetorial com `ChromaDB` e embeddings do modelo `e5-small`.

---

## 🧱 4. Dificuldades Enfrentadas

- As respostas geradas pelo agente ainda são muito genéricas ou irrelevantes.
- Embeddings parecem fracos — o sistema não está encontrando os trechos certos.
- Chunking inicial quebrou cláusulas no meio, perdendo contexto.
- Dúvida se estamos incluindo metadados corretamente no `ChromaDB`.

---

## 🛠️ 5. Estratégias de Superação

- Ajustamos o chunking para considerar hierarquia de headings no `.docx`.
- Testamos usar o `e5-base` no lugar do `e5-small`, mas não tivemos ganho significativo.
- Fizemos logging dos documentos retornados na busca vetorial para entender o que está vindo.

---

## 🎯 6. Próximos Passos

- Reestruturar os documentos com um parser mais robusto que preserve cláusulas inteiras.
- Criar uma função de avaliação da resposta baseada em "overlap" com o trecho encontrado.
- Testar uma alternativa de reranking dos trechos antes de enviar à LLM.

---

## 📢 7. Pedido de Ajuda

- Precisamos de ajuda para definir uma boa estratégia de chunking em documentos jurídicos.
- Também gostaríamos de saber se vale a pena testar outros modelos de embedding (e quais seriam gratuitos e compatíveis).

---
