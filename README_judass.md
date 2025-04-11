# Projeto: Judass - Assistente Jurídico Inteligente

## 👨‍🎓 Integrantes
- Ana Beatriz Lima
- Carlos Henrique Souza
- Diego Martins

## 💡 Ideia Principal
Criar um assistente jurídico inteligente que utiliza modelos de linguagem (LLMs) e técnicas de RAG (Retrieval-Augmented Generation) para responder perguntas com base em documentos legais fornecidos.

## 🎯 Objetivos
- Automatizar o atendimento a dúvidas jurídicas simples com base em documentos reais.
- Reduzir o tempo de resposta para advogados e clientes.
- Criar uma interface consultiva segura e contextualizada para escritórios jurídicos.

## 👥 Público-Alvo
- Escritórios de advocacia de pequeno e médio porte.
- Departamentos jurídicos de empresas.
- Estudantes de Direito que precisam revisar jurisprudências e leis.

## 🤖 Agentes Envolvidos
- **Agente Ingestor de Documentos**: processa e indexa arquivos (PDF, DOC, TXT) em uma base vetorizada.
- **Agente Consultor LLM**: responde perguntas com base nos documentos relevantes recuperados.
- **Agente Interface Web**: recebe perguntas do usuário e apresenta as respostas.

## 🧱 Tecnologias Pretendidas
- `Python`
- `LangChain` para orquestração dos agentes
- `ChromaDB` ou `FAISS` para a base vetorial
- `OpenAI GPT-3.5` ou `Google FLAN-T5` como modelo LLM
- `Streamlit` para interface simples

> As ferramentas foram escolhidas por sua integração facilitada com RAG, documentação acessível e bom suporte para prototipagem rápida.

## 📦 Entradas e Saídas Esperadas
**Entradas:**
- Arquivos legais (PDF, textos)
- Perguntas em linguagem natural

**Saídas:**
- Respostas contextuais baseadas nos documentos
- Trechos dos documentos usados como justificativa

## 🔁 Interação entre os Agentes
1. O usuário envia documentos legais para o sistema.
2. O agente ingestor processa e armazena em uma base vetorial.
3. O usuário faz uma pergunta.
4. O agente consultor busca documentos relevantes e os envia ao LLM.
5. O LLM responde com base no conteúdo e mostra a fonte.

## 🗂️ Organização e Planejamento do Projeto
O progresso deste projeto será monitorado através do **GitHub Projects**.

> Acesse a aba "Projects" do repositório para acompanhar:
- Tarefas pendentes
- Tarefas em andamento
- Tarefas concluídas

Cada integrante deve ser responsável por pelo menos uma tarefa no quadro.
Use etiquetas (labels) e comentários para detalhar o andamento e as decisões.

## 📌 Status Inicial do Projeto
- [ ] Ideia discutida e validada com o professor
- [ ] Estrutura básica do repositório criada
- [ ] Quadro no GitHub Projects criado
- [ ] Primeiras tarefas definidas e atribuídas

## 📄 Documentação Futura
Este repositório poderá incluir:
- Diagrama de arquitetura dos agentes
- Exemplo de consulta real
- Relatórios de testes com usuários
- Métricas de acurácia das respostas

## 👨‍🏫 Acompanhamento pelo Professor
Para que o professor possa acompanhar e orientar o andamento do projeto, **adicione o usuário `igorbarcosta` como colaborador do repositório.**

### Como fazer:
1. Vá até a aba **"Settings"** do seu repositório.
2. Clique em **"Collaborators"** no menu lateral.
3. Digite o nome de usuário: `igorbarcosta`
4. Clique em **"Add collaborator"** e confirme.
