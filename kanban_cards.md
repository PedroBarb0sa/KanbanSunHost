# SunHost Floripa - Quadro Kanban/Scrum

**Projeto:** SunHost Floripa - Plataforma de Hospedagem Colaborativa  
**Data de Criação:** 24 de Outubro de 2025  
**Modelo:** Kanban/Scrum v1.2  
**Responsável:** Product Owner & Stakeholders  

---

## 📋 ESTRUTURA DO QUADRO

### Listas (Colunas):
1. **BACKLOG** - Todos os cartões definidos pelo PO
2. **SPRINT BACKLOG** - Cartões prioritários para desenvolvimento
3. **TO DO ANÁLISE DE REQUISITOS** - Cartões em análise pelo Líder de Equipe
4. **TO DO** - Cartões em desenvolvimento
5. **SPRINT REVIEW** - Cartões para revisão do PO/Stakeholder
6. **IMPEDIMENTOS** - Cartões bloqueados
7. **PRONTOS** - Cartões concluídos

---

## 🎯 CARTÕES (USER STORIES)

### **CARTÃO 1: US-1 - Cadastro de Anfitrião/Hóspede**

**Status:** SPRINT BACKLOG  
**Prioridade:** 🔴 Prioritário  
**Esforço:** 🟡 Médio  
**Sprint:** Sprint 1  
**Épico:** Onboarding & Autenticação

**Título Completo:**  
_"Como Anfitrião ou Turista, eu quero me cadastrar na plataforma SunHost Floripa para criar meu perfil e começar a usar os serviços."_

**Descrição Detalhada:**  
O sistema deve permitir que novos usuários (Anfitriões e Turistas) se cadastrem na plataforma através de um formulário de cadastro. O formulário deve coletar dados pessoais (nome, email, telefone), de contato e, especificamente para anfitriões, informações sobre o imóvel (localização, tipo, etc.). Após o cadastro, um perfil de usuário é criado, permitindo que anfitriões listem seus imóveis e turistas busquem e reservem acomodações.

**Persona:** Ana (Anfitriã Local) / Turista Consciente  
**Ambiente:** Plataforma SunHost Floripa (web/mobile)  
**Objeto:** Formulário de cadastro

**Atividades Estratificadas (CheckList):**
- [ ] Design da tela de cadastro (Web & Mobile)
- [ ] Desenvolvimento do formulário (Frontend)
- [ ] Validação de dados (Frontend & Backend)
- [ ] Integração com banco de dados (Backend)
- [ ] Autenticação e geração de token (Backend)
- [ ] Testes unitários (QA)
- [ ] Testes de integração (QA)
- [ ] Documentação da API (Documentação)

**Membros:** Product Owner, Desenvolvedor Frontend, Desenvolvedor Backend, QA  
**Data de Entrega:** Sprint 1 (Estimado)

---

### **CARTÃO 2: US-2 - Listagem de Imóveis**

**Status:** SPRINT BACKLOG  
**Prioridade:** 🔴 Prioritário  
**Esforço:** 🟡 Médio  
**Sprint:** Sprint 1  
**Épico:** Gerenciamento de Imóveis

**Título Completo:**  
_"Como Anfitrião, eu quero listar meus imóveis na plataforma SunHost Floripa para que turistas possam encontrá-los e reservá-los."_

**Descrição Detalhada:**  
O Anfitrião deve ter acesso a uma seção "Meus Imóveis" no painel de controle onde possa adicionar um novo imóvel, inserindo informações como descrição, fotos, preço, disponibilidade e regras da casa. Após a publicação, o imóvel fica visível para os turistas que buscam acomodações em Florianópolis.

**Persona:** Ana (Anfitriã Local)  
**Ambiente:** Painel do Anfitrião na plataforma SunHost Floripa  
**Objeto:** Seção "Meus Imóveis"

**Atividades Estratificadas (CheckList):**
- [ ] Design da seção "Meus Imóveis" (Web & Mobile)
- [ ] Desenvolvimento do formulário de cadastro de imóvel (Frontend)
- [ ] Upload de fotos (Frontend & Backend)
- [ ] Armazenamento de imagens (Backend - S3 ou similar)
- [ ] Validação de dados de imóvel (Frontend & Backend)
- [ ] Integração com banco de dados (Backend)
- [ ] Publicação e visibilidade (Backend)
- [ ] Testes unitários (QA)
- [ ] Testes de integração (QA)

**Membros:** Product Owner, Desenvolvedor Frontend, Desenvolvedor Backend, DevOps, QA  
**Data de Entrega:** Sprint 1 (Estimado)

---

### **CARTÃO 3: US-3 - Sistema de Reserva**

**Status:** SPRINT BACKLOG  
**Prioridade:** 🔴 Prioritário  
**Esforço:** 🟡 Médio  
**Sprint:** Sprint 1  
**Épico:** Core Business - Reservas

**Título Completo:**  
_"Como Turista Consciente, eu quero fazer uma reserva de acomodação selecionando as datas desejadas para confirmar minha estadia."_

**Descrição Detalhada:**  
O Turista deve poder acessar a página de um imóvel, visualizar um calendário de disponibilidade, selecionar as datas desejadas, revisar os detalhes da reserva (preço total, regras, etc.) e confirmar o pedido. Uma solicitação de reserva é enviada ao Anfitrião, e o Turista recebe uma notificação sobre o status do seu pedido.

**Persona:** Turista Consciente  
**Ambiente:** Página de um imóvel na plataforma SunHost Floripa  
**Objeto:** Calendário de disponibilidade e botão "Reservar"

**Atividades Estratificadas (CheckList):**
- [ ] Design do calendário de disponibilidade (Frontend)
- [ ] Desenvolvimento do componente de calendário (Frontend)
- [ ] Desenvolvimento da tela de revisão de reserva (Frontend)
- [ ] Integração com sistema de pagamento (Backend)
- [ ] Lógica de bloqueio de datas (Backend)
- [ ] Geração de notificação ao Anfitrião (Backend)
- [ ] Armazenamento de reserva no banco de dados (Backend)
- [ ] Testes unitários (QA)
- [ ] Testes de integração (QA)
- [ ] Testes de carga (QA)

**Membros:** Product Owner, Desenvolvedor Frontend, Desenvolvedor Backend, QA  
**Data de Entrega:** Sprint 1 (Estimado)

---

### **CARTÃO 4: US-5 - Filtros de Busca**

**Status:** SPRINT BACKLOG  
**Prioridade:** 🔴 Prioritário  
**Esforço:** 🟡 Médio  
**Sprint:** Sprint 1  
**Épico:** Busca & Descoberta

**Título Completo:**  
_"Como Turista Consciente, eu quero filtrar acomodações por datas, preço, tipo de imóvel e comodidades para encontrar a opção ideal para minha estadia."_

**Descrição Detalhada:**  
A página de busca de acomodações deve disponibilizar filtros avançados (datas, preço mínimo/máximo, tipo de imóvel, comodidades, localização, etc.). Ao aplicar um ou mais filtros, a lista de imóveis é atualizada em tempo real para exibir apenas os resultados que correspondem aos critérios selecionados, facilitando a escolha do Turista.

**Persona:** Turista Consciente  
**Ambiente:** Página de busca de acomodações na plataforma SunHost Floripa  
**Objeto:** Filtros de pesquisa

**Atividades Estratificadas (CheckList):**
- [ ] Design da interface de filtros (Frontend)
- [ ] Desenvolvimento dos componentes de filtro (Frontend)
- [ ] Implementação de busca em tempo real (Frontend & Backend)
- [ ] Otimização de queries de banco de dados (Backend)
- [ ] Indexação de campos de filtro (Backend)
- [ ] Testes de performance (QA)
- [ ] Testes unitários (QA)
- [ ] Testes de integração (QA)

**Membros:** Product Owner, Desenvolvedor Frontend, Desenvolvedor Backend, QA  
**Data de Entrega:** Sprint 1 (Estimado)

---

### **CARTÃO 5: US-7 - Notificações e Alertas**

**Status:** SPRINT BACKLOG  
**Prioridade:** 🟠 Próxima Versão  
**Esforço:** 🟡 Médio  
**Sprint:** Sprint 2  
**Épico:** Comunicação & Engajamento

**Título Completo:**  
_"Como Anfitrião ou Turista, eu quero receber notificações em tempo real sobre solicitações de reserva, confirmações, cancelamentos e mensagens para manter-me informado."_

**Descrição Detalhada:**  
O sistema deve enviar automaticamente notificações (via web, mobile e e-mail) sobre eventos importantes: novas solicitações de reserva, confirmações, cancelamentos, mensagens de outros usuários, etc. Usuários devem poder gerenciar suas preferências de notificação (canal, frequência, tipo de evento).

**Persona:** Ana (Anfitriã Local) / Turista Consciente  
**Ambiente:** Plataforma SunHost Floripa (web/mobile) e e-mail  
**Objeto:** Sistema de notificações

**Atividades Estratificadas (CheckList):**
- [ ] Design do sistema de notificações (Arquitetura)
- [ ] Desenvolvimento de serviço de notificações (Backend)
- [ ] Integração com provedor de e-mail (Backend)
- [ ] Implementação de push notifications (Frontend & Backend)
- [ ] Centro de preferências de notificação (Frontend & Backend)
- [ ] Testes unitários (QA)
- [ ] Testes de integração (QA)
- [ ] Testes de carga (QA)

**Membros:** Product Owner, Desenvolvedor Backend, Desenvolvedor Frontend, DevOps, QA  
**Data de Entrega:** Sprint 2 (Estimado)

---

### **CARTÃO 6: US-6 - Painel Administrativo**

**Status:** BACKLOG  
**Prioridade:** 🟠 Próxima Versão  
**Esforço:** 🔴 Alto  
**Sprint:** Sprint 2  
**Épico:** Gerenciamento & Controle

**Título Completo:**  
_"Como Anfitrião, eu quero acessar um painel administrativo completo para gerenciar minhas reservas, visualizar ganhos, editar informações de imóveis e comunicar-me com hóspedes."_

**Descrição Detalhada:**  
O Anfitrião deve ter acesso a um painel de controle centralizado onde possa: visualizar todas as suas reservas (passadas e futuras), gerenciar a disponibilidade, visualizar relatórios de ganhos, editar informações dos imóveis, comunicar-se com hóspedes via chat/mensagens, visualizar avaliações recebidas e gerenciar seu perfil. Este painel é uma versão expandida das funcionalidades básicas incluídas no MVP.

**Persona:** Ana (Anfitriã Local)  
**Ambiente:** Área logada da plataforma SunHost Floripa  
**Objeto:** Painel de controle do Anfitrião

**Atividades Estratificadas (CheckList):**
- [ ] Design do painel administrativo (Web & Mobile)
- [ ] Desenvolvimento da dashboard (Frontend)
- [ ] Integração com dados de reservas (Backend)
- [ ] Desenvolvimento de relatórios de ganhos (Frontend & Backend)
- [ ] Sistema de chat/mensagens (Frontend & Backend)
- [ ] Gerenciamento de disponibilidade avançado (Frontend & Backend)
- [ ] Testes unitários (QA)
- [ ] Testes de integração (QA)
- [ ] Testes de usabilidade (QA)

**Membros:** Product Owner, Desenvolvedor Frontend, Desenvolvedor Backend, UX Designer, QA  
**Data de Entrega:** Sprint 2 (Estimado)

---

### **CARTÃO 7: US-4 - Sistema de Avaliação e Review**

**Status:** BACKLOG  
**Prioridade:** 🟣 Versão Futura  
**Esforço:** 🟡 Médio  
**Sprint:** Sprint 3  
**Épico:** Reputação & Confiança

**Título Completo:**  
_"Como Anfitrião ou Turista, eu quero avaliar minha experiência (hospedagem, anfitrião, hóspede) com uma nota e comentário para construir confiança e reputação na comunidade."_

**Descrição Detalhada:**  
Após a conclusão de uma estadia, tanto o Anfitrião quanto o Turista devem poder avaliar a experiência através de um formulário de avaliação. A avaliação inclui uma nota (1-5 estrelas) e um comentário descritivo. As avaliações são publicadas no perfil do Anfitrião e do Hóspede, ajudando a construir confiança e reputação na comunidade. O sistema deve calcular uma nota média e exibir o histórico de avaliações.

**Persona:** Ana (Anfitriã Local) / Turista Consciente  
**Ambiente:** Plataforma SunHost Floripa, após a conclusão da estadia  
**Objeto:** Formulário de avaliação

**Atividades Estratificadas (CheckList):**
- [ ] Design do formulário de avaliação (Frontend)
- [ ] Desenvolvimento do formulário (Frontend)
- [ ] Lógica de cálculo de nota média (Backend)
- [ ] Armazenamento de avaliações (Backend)
- [ ] Exibição de avaliações no perfil (Frontend & Backend)
- [ ] Moderação de avaliações (Backend)
- [ ] Testes unitários (QA)
- [ ] Testes de integração (QA)

**Membros:** Product Owner, Desenvolvedor Frontend, Desenvolvedor Backend, Moderador, QA  
**Data de Entrega:** Sprint 3 (Estimado)

---

## 📊 RESUMO DE PRIORIZAÇÃO

| User Story | Prioridade | Sprint | Esforço | Status |
| :--- | :---: | :---: | :---: | :--- |
| US-1: Cadastro | 🔴 Prioritário | Sprint 1 | Médio | SPRINT BACKLOG |
| US-2: Listagem de Imóveis | 🔴 Prioritário | Sprint 1 | Médio | SPRINT BACKLOG |
| US-3: Sistema de Reserva | 🔴 Prioritário | Sprint 1 | Médio | SPRINT BACKLOG |
| US-5: Filtros de Busca | 🔴 Prioritário | Sprint 1 | Médio | SPRINT BACKLOG |
| US-7: Notificações | 🟠 Próxima Versão | Sprint 2 | Médio | SPRINT BACKLOG |
| US-6: Painel Admin | 🟠 Próxima Versão | Sprint 2 | Alto | BACKLOG |
| US-4: Avaliação/Review | 🟣 Versão Futura | Sprint 3 | Médio | BACKLOG |

---

## 🔗 Etiquetas Utilizadas

- **Prioridade:** Prioritário, Próxima Versão, Versão Futura
- **Esforço:** Alto, Médio, Baixo
- **Sprint:** Sprint 1, Sprint 2, Sprint 3
- **Épico:** Onboarding & Autenticação, Gerenciamento de Imóveis, Core Business - Reservas, Busca & Descoberta, Comunicação & Engajamento, Gerenciamento & Controle, Reputação & Confiança

---

**Última Atualização:** 24 de Outubro de 2025  
**Versão do Modelo:** Kanban/Scrum v1.2

