# 🚀 Tutorial: Introdução ao Microsoft Azure e à Computação em Nuvem

## 📌 Objetivo

Este guia tem como objetivo apresentar os conceitos fundamentais da **computação em nuvem** e um passo a passo prático para começar a usar o **Microsoft Azure**.

---

## ☁️ Parte 1: Conceitos Básicos de Computação em Nuvem

### 🌥️ O que é Computação em Nuvem?

Computação em nuvem é a entrega de recursos de TI (como servidores, armazenamento, bancos de dados, redes e software) pela internet (“a nuvem”), com pagamento conforme o uso.

### 🧩 Modelos de Serviço

| Modelo | Descrição | Exemplo |
|--------|-----------|---------|
| IaaS (Infraestrutura como Serviço) | Recursos de infraestrutura virtualizados. | Máquinas virtuais, redes |
| PaaS (Plataforma como Serviço) | Ambiente para desenvolvimento sem gerenciar infraestrutura. | Azure App Service |
| SaaS (Software como Serviço) | Software pronto acessado via navegador. | Microsoft 365, Gmail |

### 🏗️ Modelos de Implantação

| Tipo | Descrição |
|------|-----------|
| Nuvem Pública | Recursos são hospedados por um provedor como o Azure. |
| Nuvem Privada | Recursos usados exclusivamente por uma organização. |
| Nuvem Híbrida | Combinação de nuvem pública e privada. |

---

## 🔑 Parte 2: Características Essenciais da Computação em Nuvem

Segundo o NIST (National Institute of Standards and Technology), a nuvem possui cinco características principais:

1. **Autoatendimento sob demanda** – Usuários podem provisionar recursos automaticamente, sem intervenção humana.
2. **Acesso amplo à rede** – Recursos estão disponíveis pela internet e acessíveis por múltiplas plataformas.
3. **Agrupamento de recursos (resource pooling)** – Recursos físicos e virtuais são compartilhados e alocados dinamicamente.
4. **Elasticidade rápida** – Capacidade de escalar para cima ou para baixo conforme a demanda.
5. **Serviço mensurável** – Consumo de recursos é monitorado e faturado por uso.

---

## 🔐 Parte 3: Segurança na Nuvem

### Princípios de Segurança

- **Confidencialidade**: proteção contra acesso não autorizado.
- **Integridade**: garantia de que os dados não foram alterados indevidamente.
- **Disponibilidade**: os dados e sistemas estão acessíveis quando necessário.

### Ferramentas e Boas Práticas

- Autenticação multifator (MFA)
- Criptografia em trânsito e em repouso
- Gerenciamento de identidades com Azure Active Directory (AAD)
- Controle de acesso baseado em funções (RBAC)

---

## 📈 Parte 4: Escalabilidade, Resiliência e Alta Disponibilidade

### Escalabilidade

- **Vertical (Scale Up)**: aumentar recursos de uma instância (CPU, RAM)
- **Horizontal (Scale Out)**: adicionar mais instâncias para dividir a carga

### Resiliência

Capacidade de se recuperar de falhas. Implementada com:
- Zonas de disponibilidade
- Réplicas geográficas
- Backups automáticos

### Alta Disponibilidade

Garantia de que um serviço estará disponível a maior parte do tempo (ex: 99.99%). Usada com balanceadores de carga, failover, e replicação.

---

## 📦 Parte 5: Contêineres e Serverless

### Docker e Kubernetes

- **Contêineres**: unidades leves de software que empacotam aplicação + dependências
- **Azure Kubernetes Service (AKS)**: orquestrador para implantar e gerenciar contêineres em escala

### Computação Serverless

Execução de código sem necessidade de provisionar ou gerenciar servidores. Ideal para cargas event-driven.

- **Azure Functions**: execução de funções sob demanda
- **Logic Apps**: automação baseada em workflows

---

## 🔐 Parte 6: Criando uma Conta no Azure

1. Acesse: [https://azure.microsoft.com/](https://azure.microsoft.com/)
2. Clique em **"Comece gratuitamente"**
3. Faça login com uma conta Microsoft
4. Forneça os dados necessários e aceite os termos
5. Você receberá **US$ 200 em crédito** gratuito por 30 dias

---

## 🧭 Parte 7: Navegando pelo Portal do Azure

- Acesse: [https://portal.azure.com](https://portal.azure.com)
- Principais elementos da interface:
  - **Dashboard**: Visão geral personalizável
  - **Barra de Pesquisa**: Busque qualquer recurso
  - **Todos os Serviços**: Catálogo completo de serviços
  - **Azure Marketplace**: Soluções prontas e integradas

---

## ⚙️ Parte 8: Criando sua Primeira Máquina Virtual (VM)

### Passo a Passo

1. No menu esquerdo, vá em **Máquinas Virtuais** > **Criar**
2. Configure os seguintes campos:
   - Grupo de recursos: `MeuGrupo1`
   - Nome da VM: `MinhaVM`
   - Região: Escolha a mais próxima
   - Imagem: `Ubuntu 20.04 LTS` (ou Windows)
   - Tamanho: `Standard B1s` (gratuito para testes)
   - Autenticação: usuário e senha
3. Clique em **"Revisar + Criar"** e depois em **"Criar"**

### Conectando-se à VM

- Para Linux:
  - bash
ssh usuario@ip_da_vm

 - Para Windows:

   - Use RDP ou o cliente de Área de Trabalho Remota

---

## 🧰 Parte 9: Ferramentas e Serviços Principais do Azure

### 💾 Azure Storage

Serviço de armazenamento escalável e seguro. Oferece suporte a:

- **Blobs**: arquivos grandes, como imagens, vídeos e backups
- **File Shares**: compartilhamento de arquivos entre VMs
- **Queues**: troca de mensagens entre componentes de aplicativos
- **Tables**: armazenamento NoSQL simples e rápido

### 🗃️ Azure SQL Database

Banco de dados relacional como serviço (DBaaS), altamente disponível, seguro e escalável.

**Recursos:**

- Backup automático
- Alta disponibilidade integrada
- Escalabilidade sob demanda
- Compatível com T-SQL (Transact-SQL)

### 🌐 Azure App Service

Serviço gerenciado para hospedagem de aplicativos web e APIs.

**Principais recursos:**

- Suporte a várias linguagens (.NET, Node.js, Java, PHP, Python)
- Deploy automatizado via GitHub ou Azure DevOps
- Escalabilidade automática
- Integração com certificados SSL/TLS

### 📈 Azure Monitor

Ferramenta de observabilidade que coleta, analisa e age com base em métricas e logs.

- Coleta de métricas e telemetria de desempenho
- Alertas baseados em condições personalizadas
- Dashboard de visualização e análise com Azure Log Analytics

### 🔒 Azure Active Directory (AAD)

Sistema de gerenciamento de identidade e acesso (IAM) da Microsoft.

- Autenticação e autorização segura
- Integração com Single Sign-On (SSO)
- Suporte a políticas de acesso condicional
- Integração com MFA (autenticação multifator)

---

## 🌐 Parte 10: Hospedando um Site Estático no Azure

### 🛠️ Criando uma Conta de Armazenamento

1. Vá para **Contas de Armazenamento** no portal Azure
2. Clique em **Criar**
3. Escolha o nome, região e tipo de redundância
4. Após criada, acesse a conta e vá em **Contêineres**
5. Crie um contêiner chamado `site` com acesso público

### 🌍 Habilitando Site Estático

1. Na conta de armazenamento, clique em **Site Estático (Static Website)**
2. Ative o serviço e configure:
   - Documento de índice: `index.html`
   - Documento de erro (opcional): `404.html`
3. Copie a **URL do site estático** gerada

### 📤 Fazendo Upload dos Arquivos

1. Acesse o contêiner `site`
2. Faça upload dos arquivos HTML, CSS e JS
3. Acesse o site via a URL pública fornecida

---

## 💸 Parte 11: Monitoramento e Custos

### 🔍 Azure Cost Management + Billing

Ferramenta integrada para visualizar, gerenciar e otimizar custos:

- Relatórios detalhados de consumo
- Orçamentos com notificações por e-mail
- Estimativas futuras com base no uso atual
- Exportação de dados em CSV

### 💡 Dicas para evitar custos desnecessários

- Use recursos gratuitos no plano "Free Tier"
- Desligue ou exclua recursos não utilizados (como VMs)
- Configure alertas de orçamento
- Use políticas de governança com Azure Policy

---

## 🎓 Parte 12: Recursos para Aprendizado

Aprenda mais com os materiais oficiais da Microsoft:

- [Microsoft Learn – Azure](https://learn.microsoft.com/azure/)
- [Certificações Microsoft](https://learn.microsoft.com/certifications/)
  - AZ-900 (Fundamentos)
  - AZ-104 (Administrador)
  - AZ-204 (Desenvolvedor)
- [Microsoft Docs](https://learn.microsoft.com/)
- [Canal do Azure no YouTube](https://www.youtube.com/user/windowsazure)

---

## ✅ Conclusão

Com este guia, você:

- Compreendeu os principais **conceitos da computação em nuvem**
- Aprendeu a criar e gerenciar recursos no **Microsoft Azure**
- Conheceu serviços essenciais como VMs, App Services, Storage e SQL
- Explorou conceitos avançados como **serverless, containers, segurança e escalabilidade**

Aproveite para praticar, testar novos serviços e evoluir suas habilidades em nuvem! 🌐🚀

---

**Licença:** Este conteúdo é livre para uso educacional e não possui restrições comerciais.  
Criado com 💙 para aprendizes de nuvem.

