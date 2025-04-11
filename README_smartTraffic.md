# Projeto: SmartTraffic IA

## 👨‍🎓 Integrantes
- João Silva
- Maria Oliveira
- Lucas Santos

## 💡 Ideia Principal
Desenvolver um sistema inteligente de controle de tráfego em cruzamentos urbanos, utilizando agentes autônomos em cada semáforo que aprendem com base nos fluxos de veículos por meio de aprendizado por reforço.

## 🎯 Objetivos
- Reduzir o tempo de espera dos veículos nos cruzamentos.
- Evitar congestionamentos locais em horários de pico.
- Criar um ambiente de simulação para testar estratégias de controle de tráfego.

## 👥 Público-Alvo
- Prefeituras e órgãos de mobilidade urbana.
- Pesquisadores em sistemas inteligentes e transporte.
- Cidades que buscam soluções acessíveis para controle de tráfego.

## 🤖 Agentes Envolvidos
- **Agente Semáforo**: decide o tempo de abertura com base no fluxo local.
- **Agente Monitor de Tráfego**: coleta dados de sensores e os envia ao semáforo.
- **Agente Coordenador Central** (opcional): supervisiona e identifica padrões globais.

## 🧱 Tecnologias Pretendidas
- `Python`
- `SUMO` (Simulation of Urban Mobility) como ambiente de simulação
- `Stable-Baselines3` para aprendizado por reforço
- `Flask` ou `FastAPI` para visualização simples das decisões

> Essas tecnologias foram escolhidas pela sua adequação à simulação de ambientes físicos e ao suporte robusto ao aprendizado por reforço.

## 📦 Entradas e Saídas Esperadas
**Entradas:**
- Número de veículos por faixa
- Tempo desde a última mudança de sinal
- Estado atual do cruzamento

**Saídas:**
- Ação do semáforo (abrir/fechar e duração)
- Logs das decisões
- Métricas de desempenho (tempo médio de espera, throughput)

## 🔁 Interação entre os Agentes
1. O agente monitor detecta o fluxo de veículos.
2. Ele envia esses dados ao agente semáforo.
3. O agente semáforo decide a próxima ação com base em uma política aprendida.
4. O agente coordenador, se existir, ajusta o comportamento global dos semáforos.

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
- Gráficos de desempenho dos agentes
- Scripts de simulação com diferentes cenários
- Relatórios de eficiência do controle semafórico

## 👨‍🏫 Acompanhamento pelo Professor
Para que o professor possa acompanhar e orientar o andamento do projeto, **adicione o usuário `igorbarcosta` como colaborador do repositório.**

### Como fazer:
1. Vá até a aba **"Settings"** do seu repositório.
2. Clique em **"Collaborators"** no menu lateral.
3. Digite o nome de usuário: `igorbarcosta`
4. Clique em **"Add collaborator"** e confirme.
