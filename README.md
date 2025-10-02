# ☁️ Guia Rápido de Conceitos de Cloud Computing

Este repositório serve como um resumo dos principais conceitos abordados em aulas sobre **Cloud Computing**. O objetivo é ter uma referência rápida e acessível para revisar tópicos essenciais.

---

## 🏗️ Modelos de Nuvem

Existem três modelos principais de implantação de serviços em nuvem, cada um com suas características e casos de uso específicos:

* **🔒 Nuvem Privada (Private Cloud):** A infraestrutura de nuvem é operada exclusivamente por uma única organização. Oferece alto nível de **segurança** e **controle**. Ideal para empresas com requisitos regulatórios rigorosos.
* **🌐 Nuvem Pública (Public Cloud):** Os serviços de computação são oferecidos por provedores como **Microsoft Azure**, AWS ou GCP. Os recursos são **compartilhados** por múltiplos clientes. É altamente escalável, flexível e econômica (pagamento por uso).
* **🔗 Nuvem Híbrida (Hybrid Cloud):** Combina nuvens públicas e privadas, permitindo que os dados e aplicações se movam entre elas. Oferece a **flexibilidade** da nuvem pública e a **segurança** da nuvem privada, otimizando custos.

---

## 💰 Comparativo: CapEx vs. OpEx

Entender a diferença entre **CapEx** (Capital Expenditure) e **OpEx** (Operational Expenditure) é fundamental para avaliar o modelo financeiro da computação em nuvem.

| Tipo | Nome | Descrição | Modelo Financeiro |
| :--- | :--- | :--- | :--- |
| **CapEx** | **Despesas de Capital** | 📉 Gasto inicial de dinheiro em **infraestrutura física** (servidores, hardware). | O valor do investimento se **reduz** (deprecia) com o tempo. |
| **OpEx** | **Despesas Operacionais** | 💸 Gastar com produtos e serviços **conforme necessário** (Pay-as-you-go/Pagamento conforme o uso). | O valor é **cobrado imediatamente** e é uma despesa recorrente. |

---

## 🧩 Tipos de Serviço de Nuvem (IaaS, PaaS, SaaS)

Os serviços de nuvem são categorizados em três modelos principais, definindo a divisão de responsabilidade entre o cliente e o provedor.

### Definições

* **IaaS (Infraestrutura como Serviço):**
    * Cria uma infraestrutura de TI de pagamento conforme o uso alugando servidores, máquinas virtuais, armazenamento, redes e sistemas operacionais de um provedor de nuvem.
* **PaaS (Plataforma como Serviço):**
    * Fornece um ambiente para a criação, o teste e a implantação de aplicativos de software, sem que o cliente precise focar no gerenciamento da infraestrutura subjacente.
* **SaaS (Software como Serviço):**
    * Os usuários se conectam e usam aplicativos baseados em nuvem pela Internet, como Microsoft Office 365, e-mail e calendários.

### Comparação do Serviço de Nuvem

| Serviço | Flexibilidade | Foco Principal | Gerenciamento de Infraestrutura | Modelo de Preço |
| :--- | :--- | :--- | :--- | :--- |
| **IaaS** | **Mais flexível** | Configuração e gerenciamento de hardware (VMs) para seu aplicativo. | Realizado principalmente pelo Cliente (SO, Runtime, Dados). | Pagamento conforme o uso. |
| **PaaS** | Moderada | **Desenvolvimento de aplicativos** e código. | Realizado pelo Provedor (SO, Rede, Servidores). | Pagamento conforme o uso. |
| **SaaS** | Menos flexível | Uso do **software** diretamente (e-mail, CRM). | Realizado pelo Provedor (Tudo, exceto os dados do usuário). | Modelo de assinatura. |

---

## 🤝 Modelo de Responsabilidade Compartilhada

O **Modelo de Responsabilidade Compartilhada** define quem é responsável por cada parte do ambiente de nuvem, dependendo do tipo de serviço (IaaS, PaaS, SaaS) utilizado.

| Componente | Nuvem (IaaS) | Nuvem (PaaS) | Nuvem (SaaS) | On-Premises |
| :--- | :---: | :---: | :---: | :---: |
| **Aplicações** | Cliente | Cliente | Provedor | Cliente |
| **Dados & Contas** | Compartilhada | Compartilhada | Compartilhada | Cliente |
| **Sistema Operacional** | Cliente | Provedor | Provedor | Cliente |
| **Controles de Rede** | Cliente | Provedor | Provedor | Cliente |
| **Rede Física** | Provedor | Provedor | Provedor | Cliente |
| **Infraestrutura Física** | Provedor | Provedor | Provedor | Cliente |

> **Nota:** A segurança da nuvem é sempre de responsabilidade do provedor (Microsoft), enquanto a segurança *na* nuvem (dados, identidade, dispositivos) é uma responsabilidade que é **compartilhada** ou totalmente do cliente.

---

## 🚀 Benefícios Essenciais da Nuvem Azure

A computação em nuvem, e especificamente o Azure, oferece uma série de benefícios que impactam diretamente a operação e o custo das empresas.

| Benefício | Descrição Rápida |
| :--- | :--- |
| **Alta Disponibilidade** | Garante tempo de atividade máximo (SLA), independentemente de falhas. |
| **Escalabilidade** | Capacidade de ajustar recursos para atender à demanda, pagando apenas pelo uso. |
| **Elasticidade** | Expansão ou contração automática (ou manual) de recursos em picos de demanda. |
| **Confiabilidade** | Infraestrutura resiliente e descentralizada, com recursos em múltiplas regiões. |
| **Previsibilidade** | Confiança no desempenho e no custo, influenciado pelo Azure Well-Architected Framework. |
| **Segurança** | Oferece ferramentas de segurança robustas, mas o cliente gerencia sua implementação. |
| **Governança** | Auditoria e conformidade automatizadas, ajudando a manter padrões corporativos. |
| **Gerenciabilidade** | Opções para gerenciar tanto os recursos da nuvem quanto o ambiente de nuvem em si. |

### 📈 Detalhamento dos Benefícios

* **🥇 Alta Disponibilidade:** Concentra-se em garantir a **disponibilidade máxima** dos serviços, garantida pelo **Nível de SLA (Service Level Agreement)**.
* **⚖️ Escalabilidade:** Capacidade de **ajustar recursos** para atender à demanda. Você paga apenas pelo que usa e pode escalar **Verticalmente** (adicionar mais CPU/RAM) ou **Horizontalmente** (adicionar mais instâncias).
* **🔄 Elasticidade:** Permite que os recursos sejam **expandidos ou contraídos automaticamente** em resposta a um salto repentino na demanda (Ex: Black Friday).
* **🛡️ Confiabilidade:** **Design descentralizado** com recursos implantados em **várias regiões globais**, garantindo resiliência contra eventos catastróficos.
* **🔮 Previsibilidade:** Confiança no **desempenho** e no **custo**, baseada nas diretrizes do **Microsoft Azure Well-Architected Framework**.
* **🔒 Segurança:** Oferece ferramentas de segurança. Em **IaaS**, o controle máximo é do cliente (incluindo *patching*). Em **PaaS/SaaS**, o *patching* é automático do provedor.
* **🏛️ Governança:** **Auditoria baseada em nuvem** para sinalizar recursos fora de conformidade e aplicação automática de patches para manter a segurança.
* **🛠️ Gerenciabilidade:** Oferece **Gerenciamento *da* Nuvem** (escalar e implantar recursos) e **Gerenciamento *na* Nuvem** (gerenciar via Portal, CLI, APIs, PowerShell).

---

## 💻 Configuração de Recursos no Azure

### Criação de Máquinas Virtuais (VMs)

A criação de uma Máquina Virtual (VM) é um recurso de **IaaS (Infraestrutura como Serviço)**.

**🗺️ Caminho Simplificado no Portal:**

`Portal Azure` &rarr; `Todos os serviços` &rarr; `Computação` &rarr; `Máquinas Virtuais` &rarr; `Criar` &rarr; `Máquina virtual do Azure`

> **Referência:** [Criar uma máquina virtual Windows no portal do Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)

### Configurando uma Instância de Banco de Dados

A configuração de um Banco de Dados Gerenciado (como o Azure SQL Managed Instance) é um exemplo de serviço **PaaS (Plataforma como Serviço)**, pois a infraestrutura subjacente é gerenciada pelo Azure.

> **Referência:** [Criar uma instância gerenciada do Azure SQL](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart?view=azuresql&tabs=azure-portal)

---

Este README será atualizado à medida que novas aulas forem concluídas.
