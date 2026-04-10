# RFC: Request for Comments — Projeto de Portfólio

**Engenharia de Software – Católica SC**

---

# Identificação

- **Título do Projeto:**  
  Nome claro e específico do sistema.

- **Linha de Projeto (Direction):**  
  Web

- **Autor:**  
  Lucas Affonso Klemke

- **Data da Proposta:**  
  11/04/2026

- **Versão:**  
  1.0

---

# 1. Visão do Produto e Impacto (O Problema)

O objetivo desta seção é responder uma pergunta fundamental:

**Este projeto resolve um problema real ou é apenas um exercício técnico?**

---

## 1.1 Contexto e Problema

O advogado Dr. Lucas Quintino é o principal afetado pelo problema, que ocorre no contexto da rotina diária do seu escritório, durante a gestão de clientes e o acompanhamento de processos jurídicos.

Atualmente, esse controle é feito de forma manual, utilizando planilhas, anotações pessoais e conversas dispersas no WhatsApp, sem nenhuma ferramenta centralizada.

As soluções existentes no mercado, como CRMs voltados para advocacia, apresentam alta complexidade e um volume de funcionalidades desnecessário para um advogado em início de carreira, além de representarem um custo elevado. O advogado necessita uma solução personalizada, adequada à sua realidade e às suas necessidades atuais.

---

## 1.2 Origem da Demanda e Evidências

### Demanda Externa

O projeto foi solicitado pelo escritório de advocacia do Dr. Lucas Quintino. O escritório enfrenta dificuldades na organização e centralização dos dados de clientes, no acompanhamento de atendimentos via WhatsApp e na visualização clara da etapa em que cada cliente se encontra dentro do fluxo de trabalho.

---

### Pesquisa com Usuários

![alt text](<Screenshot 2026-04-10 at 08.55.58.png>)

---

### Evidência de Interesse

![alt text](<Screenshot 2026-04-10 at 08.55.10.png>)

---

## 1.3 Análise de Soluções Existentes (Benchmark)

### 1. ADVBOX

**Link:** [advbox.com.br](https://advbox.com.br)

**Público-alvo:** Escritórios de advocacia de pequeno a grande porte.

**Funcionalidades principais:** Gestão de processos, CRM jurídico com kanban, controle de prazos e intimações, financeiro integrado, produtividade por equipe (método Taskscore) e inteligência artificial.

**Preço:** A partir de R$180/mês (plano Essencial) podendo chegar a R$1.200/mês (plano Elite).

**Limitações:** Voltado para escritórios que já possuem volume considerável de processos, com muitas funcionalidades que um advogado iniciante não utilizaria, gerando complexidade e custo desnecessários.

---

### 2. Kommo

**Link:** [kommo.com](https://www.kommo.com)

**Público-alvo:** Pequenas e médias empresas de diversos segmentos.

**Funcionalidades principais:** CRM focado em comunicação via mensageiros, com integração nativa ao WhatsApp, Instagram, Facebook e outros canais, funil de vendas visual e automações.

**Preço:** A partir de US$15 por usuário/mês, cobrado em dólar.

**Limitações:** Não é específico para o contexto jurídico, a cobrança em dólar gera imprevisibilidade de custos, e algumas automações podem ser difíceis de configurar para usuários sem experiência com CRM.

---

### 3. Bitrix24

**Link:** [bitrix24.com.br](https://www.bitrix24.com.br)

**Público-alvo:** Empresas de todos os portes e segmentos.

**Funcionalidades principais:** CRM gratuito, gestão de contatos, calendários, faturamento, integração com canais de comunicação, gestão de projetos e marketing.

**Preço:** Possui plano gratuito com funcionalidades básicas.

**Limitações:** Plataforma genérica com dezenas de módulos (RH, projetos, sites, marketing), o que torna a experiência confusa e sobrecarregada para um advogado que precisa apenas de gestão de clientes e comunicação via WhatsApp.

---

### Comparação

| Solução | Pontos Fortes | Limitações |
|---|---|---|
| ADVBOX | Específica para advocacia, CRM kanban, controle de prazos e intimações | Custo elevado, excesso de funcionalidades para advogados iniciantes |
| Kommo | Forte integração com WhatsApp e mensageiros, interface intuitiva | Cobrança em dólar, não é voltado para o contexto jurídico |
| Bitrix24 | Plano gratuito disponível, ampla variedade de ferramentas | Excesso de módulos, curva de aprendizado alta, interface poluída |

---

### Diferencial do Projeto

As soluções existentes são voltadas para escritórios já estruturados ou para empresas de outros segmentos, apresentando excesso de funcionalidades, complexidade de configuração e custos incompatíveis com a realidade de um advogado em início de carreira que atua sozinho. O projeto proposto preenche essa lacuna ao oferecer um CRM simples, personalizado e com integração direta ao WhatsApp, atendendo especificamente às necessidades de um advogado individual que precisa apenas organizar seus clientes, visualizar o andamento dos casos e centralizar sua comunicação, sem complexidade ou custos desnecessários.

## 1.4 Público-Alvo

O público-alvo do sistema é o próprio advogado titular do escritório, Dr. Lucas Quintino, 28 anos, que atua de forma individual na gestão dos seus clientes e processos. O uso do sistema ocorrerá no dia a dia do escritório, principalmente para organizar atendimentos e acompanhar o andamento dos casos. Não é esperado conhecimento técnico avançado, portanto a interface deve ser intuitiva e de fácil utilização.

---

## 1.5 Objetivos do Projeto

### Objetivo Geral

Desenvolver um CRM personalizado com integração ao WhatsApp para centralizar a gestão de clientes e automatizar tarefas operacionais do escritório de advocacia, permitindo que o advogado tenha controle total sobre seus atendimentos de forma simples e eficiente.

---

### Objetivos Específicos

1. Centralizar o cadastro e o histórico de interações dos clientes em uma única plataforma, eliminando o uso de planilhas e anotações dispersas.
2. Integrar o sistema ao WhatsApp para registrar e organizar automaticamente as conversas com os clientes dentro do CRM.
3. Implementar um pipeline visual (kanban) que permita ao advogado identificar rapidamente em qual etapa cada cliente se encontra no fluxo de atendimento.
4. Automatizar tarefas repetitivas como lembretes de prazos, follow-ups e notificações de acompanhamento processual.
5. Fornecer uma interface simples e intuitiva, adequada a um usuário sem conhecimento técnico avançado.

---

## 1.6 Métricas de Sucesso (KPIs)

- O advogado conseguir localizar qualquer informação de um cliente em menos de 30 segundos, sem precisar consultar fontes externas ao sistema.
- As mensagens do WhatsApp serem registradas automaticamente no CRM, eliminando a necessidade de transcrição manual.
- O tempo gasto com tarefas administrativas repetitivas (lembretes, follow-ups, atualizações de status) ser reduzido em pelo menos 50% em relação ao fluxo atual.
- O advogado conseguir visualizar o status de todos os seus clientes ativos em uma única tela, sem necessidade de navegação complexa.
- O sistema ser utilizável de forma autônoma após um breve treinamento inicial, sem necessidade de suporte técnico recorrente.