# Projeto: docIA - Automação Inteligente de Documentos

## 👨‍🎓 Integrantes
- Larissa Fernandes
- Pedro Cunha
- Tiago Rocha

## 💡 Ideia Principal
Criar um sistema de automação de processos administrativos que monitora conversas em canais como WhatsApp e e-mail, identifica documentos recebidos, classifica automaticamente e os organiza em pastas corretas para diferentes setores.

## 🎯 Objetivos
- Automatizar o recebimento e a organização de documentos enviados por clientes.
- Reduzir erros humanos na triagem de arquivos.
- Aumentar a produtividade de escritórios que lidam com muitos documentos diários.

## 👥 Público-Alvo
- Cartórios e escritórios de advocacia
- Departamentos administrativos de escolas, hospitais e empresas
- Pequenas empresas que usam WhatsApp como canal de atendimento

## 🤖 Agentes e Componentes Envolvidos
- **Agente Monitor de Comunicação**: escuta mensagens de canais como WhatsApp, e-mail ou Telegram.
- **Agente Classificador de Documentos**: analisa o conteúdo e classifica o tipo de documento (RG, CPF, comprovante, etc.).
- **Agente Organizador de Pastas**: move o arquivo para o local correto dentro da estrutura de pastas do servidor.
- **Interface de Configuração**: permite cadastrar novos tipos de documentos, palavras-chave e regras.

## 🧱 Tecnologias Pretendidas
- `Python`
- `yagmail` ou `imaplib` para leitura de e-mails
- `pywhatkit` ou `Twilio API` para integração com WhatsApp
- `Tesseract OCR` para leitura de texto em imagens
- `Regex`, `spaCy` ou `scikit-learn` para classificação simples de conteúdo
- `watchdog` para monitorar arquivos e mover dinamicamente

> As tecnologias foram escolhidas por serem leves, bem documentadas e com grande potencial de integração.

## 📦 Entradas e Saídas Esperadas
**Entradas:**
- Mensagens com anexos de imagem ou PDF
- Palavras-chave nos textos de mensagens

**Saídas:**
- Documento salvo em uma pasta adequada (ex: /clientes/joao/documentos/cpf.pdf)
- Log do processo de classificação

## 🔁 Interação entre os Agentes
1. O agente monitor detecta um novo anexo em mensagem.
2. O agente classificador analisa o conteúdo do arquivo.
3. O agente organizador move o arquivo para a pasta correta.
4. Um log é gerado e a interface registra a ação.

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
- Exemplos de documentos reconhecidos
- Logs de teste com diferentes tipos de mensagem
- Relatório de desempenho do sistema
- Interface para parametrização de regras

## 👨‍🏫 Acompanhamento pelo Professor
Para que o professor possa acompanhar e orientar o andamento do projeto, **adicione o usuário `igorbarcosta` como colaborador do repositório.**

### Como fazer:
1. Vá até a aba **"Settings"** do seu repositório.
2. Clique em **"Collaborators"** no menu lateral.
3. Digite o nome de usuário: `igorbarcosta`
4. Clique em **"Add collaborator"** e confirme.
