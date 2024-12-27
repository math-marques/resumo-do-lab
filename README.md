# resumo-do-lab
Atividade do módulo de COmputação na nuvem - AZ900 -> resumo dos conceitos

# ☁️ Resumo do Módulo de Computação na Nuvem com Azure ☁️
E aí, devs! 😎 Aqui vai o resumo direto do que rolou no módulo de computação na nuvem, com aquele foco no Azure pra AZ-900, a certificação da Microsoft e também para o dia a dia do mercado nas diversas empresas que utilizam dessa solução para um bom custo-benefício de não ter uma sala gelada e vários espaços pra guardar informações.


# O que é Computação na Nuvem?
É quando você usa recursos de TI como servidores, armazenamento, banco de dados e outros serviços via internet em vez de depender de equipamentos locais. Ideal pra escalar rápido e economizar com infraestrutura física. Nada de gastar uma grana com a famosa salinha gelada. 💻➡️☁️

# Modelos de Serviço:

# IaaS (Infrastructure as a Service):
--> Você gerencia servidores virtuais, armazenamento, rede e sistemas operacionais. Ex: criar e configurar máquinas virtuais no Azure.
# PaaS (Platform as a Service):
--> Aqui o foco é no desenvolvimento. Você cria e gerencia apenas o código, enquanto o Azure cuida do ambiente, banco de dados e hospedagem.
# SaaS (Software as a Service):
--> Tudo prontinho e gerenciado. Você só acessa e usa o software pela web. Exemplo clássico: Microsoft 365.

# Modelos de Implantação:
Nuvem Pública: Infraestrutura compartilhada entre vários usuários. 
Exemplo: Azure.
Nuvem Privada: Criada exclusivamente pra uma organização, com maior controle.
Nuvem Híbrida: Combinação de pública e privada, pra maior flexibilidade.

# Por que usar Azure? Qual relevância?
Acredito que tenha ficado claro só com a abordagem de não ter algo físico e rudimentar. Mas vou destrinchar mais alguns pontos:

--> Infraestrutura Global:
Azure tem data centers espalhados pelo mundo todo, oferecendo latência baixa, alta disponibilidade e backups redundantes. 🌍

--> Custo Efetivo:
Modelo "Pay as You Go" (pague apenas pelo que usar), sem necessidade de grandes investimentos iniciais em hardware.

--> Alta Confiabilidade:
Garantia de SLA (acordo de nível de serviço) com uptime de até 99,95%.

--> Segurança e Compliance:
Infraestrutura segura, com certificações globais de conformidade e criptografia ponta a ponta.

# Serviços Chave do Azure 🔑
# 1. Compute (Poder de processamento)
Azure Virtual Machines (VMs):
Crie e gerencie máquinas virtuais Windows e Linux. Ideal pra rodar aplicativos e simular ambientes locais.
App Services:
Plataforma gerenciada pra criar, implantar e escalar aplicativos web. Sem dor de cabeça com infraestrutura.
Azure Kubernetes Service (AKS):
Gerenciamento completo de containers e orquestração usando Kubernetes.
# 2. Armazenamento
Armazenamento Blob:
Pra guardar grandes volumes de dados não estruturados, como arquivos, imagens e backups.
Discos Gerenciados:
Solução de armazenamento persistente para VMs, com escalabilidade e redundância.
Armazenamento de Arquivos (File Storage):
Compartilhamento de arquivos acessível via SMB, integrado com servidores locais.
# 3. Rede
Virtual Network (VNet):
Configure redes privadas no Azure pra conectar recursos de forma segura.
Azure Load Balancer:
Equilibre o tráfego entre instâncias de VMs ou serviços, garantindo disponibilidade.
VPN Gateway:
Crie conexões seguras entre data centers locais e a nuvem.
# 4. Banco de Dados
Azure SQL Database:
Banco de dados relacional como serviço, otimizado pra desempenho e escalabilidade.
Azure Cosmos DB:
Banco de dados NoSQL distribuído globalmente, com baixa latência.
Banco de Dados Gerenciado para PostgreSQL/MySQL:
Soluções open-source gerenciadas pelo Azure, prontas pra uso.
# 5. Segurança
Azure Security Center:
Ferramenta que analisa suas configurações e sugere melhorias na segurança.
Azure Active Directory (AAD):
Controle de acesso e identidade, com suporte a autenticação multifator e integração com apps.
Key Vault:
Armazene e gerencie chaves de criptografia, segredos e certificados de forma segura.
# 6. Gerenciamento e Monitoramento
Azure Monitor:
Fique de olho na saúde e desempenho dos seus recursos, com métricas e alertas.
Azure Resource Manager (ARM):
Modelo de gerenciamento pra organizar e implementar recursos como templates reutilizáveis.
Azure Cost Management:
Monitore e controle seus gastos no Azure, com insights detalhados.


# Observações adicionais:
Azure Free Tier: Ideal pra quem tá começando. Oferece créditos grátis (US$ 200 nos primeiros 30 dias) e serviços gratuitos por 12 meses.
CLI do Azure: Ferramenta de linha de comando pra gerenciar recursos direto do terminal. Dá pra automatizar muita coisa!
Documentação e Treinamentos: O Azure tem uma documentação super completa e vários tutoriais oficiais pra te ajudar a aprender rápido. O que mais admiro na Microsoft é a comunidade e suporte oferecido pra quem está no learning.
# AZ-900 🏅
Pretensão é tirar a certificação em 2025. Mas, entendi bem que os modelos de serviço e implantação são pontos cruciais pra prova. Praticar identificar qual serviço resolve qual problema. Usar a prática gratuita pra testar coisas como VMs, App Services e banco de dados.
Resumindo: Explorar o Azure Portal, CLI e Azure Docs.

# 🚀 Guia Ligeiro: Criação de Máquinas Virtuais no Azure ☁️  

Aprendendo a criar e configurar Máquinas Virtuais (VMs) no Azure? Esse aqui é um guia básico pra o dia a dia ou no exame AZ-900.  

---

# O que é uma VM no Azure?  
Uma VM (Virtual Machine) é um computador virtual que roda no Azure, podendo ser configurado com sistemas operacionais, aplicações e recursos customizados. E serve para testar aplicativos em diferentes ambientes (Windows/Linux), hospedar aplicações ou serviços e simular servidores locais na nuvem.  

---

# Vantagens das VMs no Azure
- **Escalabilidade**: Adicione ou remova recursos conforme a necessidade. Isso vai depender muito de cada caso. É necessário complexar e/ou facilitar seu contexto para dar certo. 
- **Custo Controlado**: Pague apenas pelo tempo de uso. E até mesmo quando for cancelar a assinatura, ele lhe envia um backup automático de tudo que tem nas mãos. É um autoserviço de ponta. 
- **Alta Disponibilidade**: Redundância em diferentes data centers.  
- **Flexibilidade**: Escolha o tamanho, região, SO e outras coisas...  

---

### **Passo a Passo pra Criar uma VM no Azure**  

#### **1️⃣ Acesse o Portal do Azure**  
- Entrar no [portal.azure.com](https://portal.azure.com) com a conta  

#### **2️⃣ Ir até "Máquinas Virtuais"**  
- No painel lateral, clicar em **Máquinas Virtuais** e, depois, em **Criar -> Máquina Virtual**.  

#### **3️⃣ Configurar os Detalhes da VM**  
- **Grupo de Recursos**: Escolher um existente ou criar um novo (é tipo uma pasta pros seus recursos).  
- **Nome da VM**: Escolher um nome único (ex: "MeuServidorDev").  
- **Região**: Escolher a localização do data center (quanto mais perto, menor a latência).  

#### **4️⃣ Escolher o Sistema Operacional**  
- **Windows**: Ideal pra aplicações como .NET ou SQL Server. É o caso indicado pra quem está mergulhando no universo Microsoft. 
- **Linux**: Melhor pra DevOps, containers, e soluções open-source.  

#### **5️⃣ Escolher o Tamanho da VM**  
- Baseado em CPU, memória e armazenamento.  
  - Exemplo:  
    - **B1s**: Básico, pra testes (custa centavos por hora).  
    - **D-Series**: Pra cargas de trabalho médias.  
    - **E-Series**: Otimizado pra aplicações com muita memória.  

#### **6️⃣ Configurar Autenticação**  
- **Usuário e Senha**: Pra Windows ou Linux (mais simples pra começar).  

#### **7️⃣ Disco e Armazenamento**  
- **SSD Premium**: Rápido, ideal pra produção.  
- **HDD Padrão**: Mais barato, bom pra ambientes de teste.  

#### **8️⃣ Rede Virtual**  
- Configuração automática cria uma **VNet** e define o acesso público pra sua VM.  
- Configure portas, como a **porta 22 (SSH)** pra Linux ou **porta 3389 (RDP)** pra Windows.  

#### **9️⃣ Revisar e Criar**  
---

### **Gerenciando sua VM**  
▶**Acesse sua VM**:  
  - Linux: Use um cliente SSH (como `PuTTY`) pra conectar via terminal.  
  - Windows: Use a Conexão de Área de Trabalho Remota (RDP).  
▶**Monitoramento**:  
  - Acompanhe consumo de CPU, memória e armazenamento pelo **Azure Monitor**.  
▶**Escalar ou Pausar**:  
  - Precisa de mais desempenho? Escale pra uma VM maior.  
  - Vai ficar um tempo sem usar? Pause pra economizar.  

---

### **Custos de VMs: Dicas pra Economizar 💰**  
1. **Tamanhos Básicos pra Testes**: Use séries como **B1s** pra ambientes simples.  
2. **Regiões Mais Baratas**: Algumas regiões (ex: Sul do Brasil) podem ser mais caras. Explore outras, como Leste dos EUA.  
3. **Pausar a VM**: Sempre desligue a VM no painel do Azure quando não estiver em uso.  
4. **Reservas de 1 ou 3 Anos**: Economize até 72% em VMs de longo prazo.  

---

### **Dicas de Ouro 🏆**  
▶ Experimente criar **Snapshots**: Faça backups rápidos do disco da sua VM.  
▶ Configure **NSG (Network Security Groups)**: Garanta que só portas necessárias estejam abertas.  
▶ Explore **Azure Bastion**: Acesse suas VMs com mais segurança, sem expor IPs públicos.  
▶ Teste com o **Azure CLI**: Automatize a criação e gerenciamento de VMs.  

---

### **VMs no Exame AZ-900**  
- Entenda os tipos de discos e tamanhos de VMs.  
- Saiba o que é VNet e portas de acesso (SSH/RDP).  
- Grave na memória o modelo de pagamento: **Pay-as-you-go**. 🌟

# ☁️ Guia Ligeiro: Configurando um Banco de Dados no Azure 🚀
Forma prática e segura de gerenciar bancos de dados na nuvem, no Azure. Ele oferece soluções completas, seja pra projetos pequenos ou grandes, com suporte a SQL Server, PostgreSQL, MySQL, e até bancos NoSQL como o Cosmos DB. Bora entender como tudo funciona?

# Por que usar bancos de dados no Azure?
---▶ Gestão simplificada: Sem dor de cabeça com hardware, backups ou atualizações;
---▶ Alta disponibilidade: Seus dados sempre acessíveis, com redundância global;
---▶ Segurança integrada: Criptografia, autenticação multifator e compliance com normas globais;
---▶ Escalabilidade: Cresceu o tráfego? O Azure ajusta os recursos automaticamente;
---▶ Conexão fácil: Integração com serviços como Azure Functions, Web Apps e Power BI;

### Tipos de Bancos Disponíveis no Azure
Azure SQL Database, PostgreSQL, MySQL, Cosmos DB, MariaDB

# Principais Recursos dos Bancos de Dados no Azure
Modos de Preço

DTU (Database Transaction Units): Simples, com recursos pré-definidos de CPU, memória e IOPS.
VCore: Controle granular pra ajustar CPU, memória e armazenamento separadamente.
Escalabilidade

Escale horizontal ou verticalmente sem interrupções.
Modelos de replicação automática, incluindo leitura global.
Segurança de Dados

Criptografia em trânsito (SSL) e em repouso (TDE - Transparent Data Encryption).
Firewalls e integração com Azure Active Directory.
Backups e Recuperação

Backups automáticos configuráveis com retenção de até 35 dias.
Recuperação ponto a ponto para evitar perda de dados.
Monitoramento e Diagnóstico


🚀 Simbora aprender sobre a nuvem e garantir um currículo legal! 💼
A meta é ir atrás do AZ-900 da microsoft

