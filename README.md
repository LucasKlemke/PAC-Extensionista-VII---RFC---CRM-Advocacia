# Capa

- **Título do Projeto**: Plataforma de Gestão de Clientes | Escritório de Advocacia Lucas Quintino.
- **Nome do Estudante**: Lucas Affonso Klemke.
- **Curso**: Engenharia de Software.
- **Data de Entrega**: [Data].

# Resumo

Este documento detalha o desenvolvimento de uma aplicação Web de gestão de clientes (CRM) para o escritório de advocacia Lucas Quintino.

## 1. Introdução

- **Contexto**: O projeto propõe o desenvolvimento de uma aplicação web CRM voltada para escritórios de advocacia, permitindo gerenciar leads, enviar mensagens via WhatsApp e gerar contratos a partir de modelos já existentes.

- **Justificativa**: A ferramenta é relevante pois centraliza atividades essenciais do relacionamento com clientes e automatiza tarefas recorrentes, tornando o processo mais ágil e organizado dentro do escritório.

- **Objetivos**: Facilitar o acompanhamento de leads, a comunicação com clientes por WhatsApp e a geração de contratos, integrando tudo em um único sistema simples e eficiente.

## 2. Descrição do Projeto

- **Linha de Projeto**: Web Apps

- **Tema do Projeto**: Desenvolvimento de uma plataforma SaaS de CRM jurídico para automação e centralização do relacionamento com clientes em escritórios de advocacia.

- **Propósito e Uso Prático**: O sistema resolve o desafio de gerenciar leads, manter clientes ativos, facilitar comunicações e gerar contratos padronizados, tudo em um único ambiente totalmente digital. Permitirá que advogados organizem contatos, historizem atendimentos e automatizem interações de pós-venda, tornando o fluxo operacional mais eficiente e rastreável.

- **Público-Alvo**: Pequenos e médios escritórios de advocacia ou profissionais autônomos do Direito que buscam modernizar a gestão do relacionamento com clientes, aumentar a retenção e profissionalizar o atendimento.

- **Problemas a Resolver**:
  - Dificuldade em controlar o fluxo de leads e clientes ao longo do tempo.
  - Falta de automação no envio de lembretes e mensagens de follow-up.
  - Processos morosos e manuais para gerar contratos e organizar o histórico de atendimentos.
  - Risco de perder clientes por ausência de contato ou organização deficiente das interações.

- **Diferenciação/Ineditismo**: 
  - Integração nativa e automatizada com WhatsApp (API não oficial Uazapi) para notificações e mensagens de reativação.
  - Geração automática de contratos a partir de modelos personalizados, eliminando retrabalho.
  - Plataforma 100% Web, responsiva e planejada para uso em dispositivos móveis e desktop, pensada para contexto jurídico nacional.
  - Isolamento total dos dados entre escritórios (“multiempresa”/multitenant) em conformidade total com a LGPD.

- **Limitações**: 
  - O sistema não realiza peticionamento ou automação de rotinas processuais em sistemas de tribunais.
  - Não contempla funções de contabilidade, folha de pagamento ou gestão financeira detalhada (limita-se a relatórios de receita bruta).
  - Não se propõe a substituir ERPs jurídicos completos, focando apenas em CRM e automações relacionadas ao atendimento do cliente.

- **Normas e Legislações Aplicáveis**:
  - LGPD (Lei Geral de Proteção de Dados) – Armazenamento seguro e consentimento para dados pessoais.
  - Código de Ética e Disciplina da OAB – Garantir comunicação ética, sem captação irregular de clientela.
  - Requisitos básicos de acessibilidade web (WCAG 2.1).
  - Eventuais restrições para utilização da API do WhatsApp conforme os termos da Meta.

- **Métricas de Sucesso**:
  - Redução média do tempo de resposta ao lead para menos de 1 hora durante horário comercial.
  - Aumento de 20% no índice de reativação de clientes inativos em 6 meses.
  - Mais de 85% das comunicações transacionadas via WhatsApp ocorrendo sem intervenção manual.
  - Taxa de geração automática de contratos acima de 90% para novos atendimentos.
  - Satisfação dos usuários medida por NPS ≥ 8,0 após três meses de uso.

## 3. Especificação Técnica

Descrição detalhada da proposta, contemplando requisitos, arquitetura, tecnologias, segurança e aderência aos critérios obrigatórios da linha de projeto escolhida.

### 3.1. Requisitos de Software
- **Requisitos Funcionais (RF)**: Liste de forma clara as funcionalidades que o sistema deverá oferecer.
- **Requisitos Não-Funcionais (RNF)**: Inclua requisitos de desempenho, segurança, usabilidade, escalabilidade, disponibilidade, entre outros.
- **Representação dos Requisitos**: Inclua um Diagrama de Casos de Uso (UML) ou outra representação visual que facilite o entendimento.
- **Aderência aos Requisitos da Linha de Projeto**: Indique como cada requisito está alinhado aos itens “Obrigatório Atender” definidos para a linha de projeto (Web, Mobile, Jogos, IA ou IoT).

### 3.2. Considerações de Design
- **Visão Inicial da Arquitetura**: Apresente os principais componentes e suas interações.
- **Padrões de Arquitetura**: Informe padrões adotados (ex.: [MVC](https://en.wikipedia.org/wiki/Model–view–controller), [Microserviços](https://microservices.io/), [MVVM](https://en.wikipedia.org/wiki/Model–view–viewmodel), Arquitetura em Camadas).
- **Modelos C4**: Utilize os quatro níveis ([C4 Model](https://c4model.com/)) quando aplicável.
- **Mockups das Telas Principais**: Apresente protótipos visuais das telas mais relevantes, mostrando navegação, disposição de elementos e principais interações do usuário. Esses mockups podem ser feitos em ferramentas como Figma, Adobe XD ou similares, e devem refletir a identidade visual e usabilidade prevista para o produto.
- **Decisões e Alternativas Consideradas**: Justifique escolhas de design, documentando alternativas avaliadas.
- **Critérios de Escalabilidade, Resiliência e Segurança**: Descreva como a solução será projetada para suportar crescimento, lidar com falhas e manter segurança.

### 3.3. Stack Tecnológica
- **Linguagens de Programação**: Escolhida para garantir uma tipagem estática rigorosa ao desenvolvimento. O objetivo principal é a redução de bugs em tempo de execução, proporcionando maior segurança no código, manutenibilidade a longo prazo e uma experiência de desenvolvimento mais fluida em comparação ao JavaScript puro.
- **Frameworks e Bibliotecas**: 
Next.js: Utilizado como o framework principal por unir os recursos modernos do React (como componentes de servidor e renderização híbrida) à eficiência de rotas de API integradas. É a escolha ideal para entregas que exigem agilidade e escalabilidade.

Tailwind CSS: Adotado para a estilização da interface, permitindo a criação de layouts responsivos e personalizados com alta velocidade de desenvolvimento através de classes utilitárias.

shadcn/ui: Utilizada em conjunto com o Tailwind para fornecer componentes modulares, acessíveis e pré-configurados. Essa biblioteca garante uma identidade visual sofisticada e evita o retrabalho na criação de elementos complexos de UI.

Prisma ORM: Atua como a camada de abstração entre o código e o banco de dados. Foi selecionado pela sua capacidade de prevenir nativamente ataques de SQL Injection, simplificar consultas complexas e realizar a gestão automatizada de migrations.

- **Ferramentas de Desenvolvimento e Gestão**: 
Cursor: Utilizado como o editor principal de código. Por ser um fork do VS Code focado em IA, ele potencializa a produtividade através de preenchimento de código contextual e refatoração inteligente, permitindo uma escrita mais rápida de componentes TypeScript e hooks do React.

Claude Code: Ferramenta de linha de comando (CLI) baseada em agente de IA para interação direta com o sistema de arquivos e o terminal, auxiliando em tarefas complexas de codificação e resolução de bugs diretamente no ambiente de desenvolvimento.

GitHub: Plataforma central para hospedagem de código e controle de versão utilizando Git. Atua como a "única fonte da verdade" do projeto, facilitando a revisão de código (Pull Requests), o rastreamento de issues e o versionamento do esquema do banco de dados gerado pelo Prisma.

Postgres...

- **Licenciamento**: Indique as licenças dos softwares e bibliotecas utilizados ([MIT](https://opensource.org/licenses/MIT), [GPL](https://www.gnu.org/licenses/gpl-3.0.html), [Apache](https://www.apache.org/licenses/), [Creative Commons](https://creativecommons.org/licenses/)).

### 3.4. Considerações de Segurança
- **Riscos Identificados**: Liste ameaças potenciais (ex.: injeção de código, vazamento de dados, falhas de autenticação).
- **Medidas de Mitigação**: Explique as ações planejadas para minimizar riscos (ex.: criptografia, controle de acesso, validação de entrada).
- **Normas e Boas Práticas Seguidas**: Cite padrões como [OWASP Top 10](https://owasp.org/www-project-top-ten/), [ISO/IEC 27001](https://www.iso.org/isoiec-27001-information-security.html), [LGPD](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/L13709.htm) ou outros aplicáveis.
- **Responsabilidade Ética**: Para projetos de IA ou manipulação de dados sensíveis, descreva como serão tratados vieses, privacidade e uso responsável ([UNESCO – Ética em IA](https://unesdoc.unesco.org/ark:/48223/pf0000380455), [OECD AI Principles](https://oecd.ai/en/ai-principles)).

### 3.5. Conformidade e Normas Aplicáveis
- Relacione todas as legislações, regulamentações e normas técnicas aplicáveis ao projeto, descrevendo brevemente como serão atendidas.
- Exemplos:
  - [LGPD – Lei Geral de Proteção de Dados](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/L13709.htm)
    - Coletar apenas dados necessários (nome, contato, dados do imóvel).
    - Evitar dados sensíveis desnecessários.
    - Solicitar consentimento explícito e exibir política de privacidade clara.
    - Permitir acesso, correção e exclusão de dados pelo usuário.
    -   ...
   
## 4. Próximos Passos

 - Descrição dos passos seguintes após a conclusão do documento, com uma visão geral do cronograma para Portfólio I e II.
 - Definição de Marcos: Estabelecer datas para entregas intermediárias e checkpoints.


## 5. Referências

### Core Frameworks & Linguagens
* **Next.js**: [https://nextjs.org/docs](https://nextjs.org/docs)
* **React**: [https://react.dev](https://react.dev)
* **TypeScript**: [https://www.typescriptlang.org/docs](https://www.typescriptlang.org/docs)

### Interface & Design System
* **Tailwind CSS**: [https://tailwindcss.com/docs](https://tailwindcss.com/docs)
* **shadcn/ui**: [https://ui.shadcn.com](https://ui.shadcn.com)
* **Lucide Icons**: [https://lucide.dev](https://lucide.dev)
* **Radix UI**: [https://www.radix-ui.com](https://www.radix-ui.com)

### Backend & Database
* **PostgreSQL**: [https://www.postgresql.org/docs](https://www.postgresql.org/docs)
* **Prisma ORM**: [https://www.prisma.io/docs](https://www.prisma.io/docs)
* **Zod (Validation)**: [https://zod.dev](https://zod.dev)
* **Supabase**: [https://supabase.com/docs](https://supabase.com/docs)

### IA & Ferramentas de Desenvolvimento
* **Cursor Editor**: [https://www.cursor.com](https://www.cursor.com)
* **Claude Code (Anthropic)**: [https://docs.anthropic.com/en/docs/agents-and-tools/claude-code](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code)
* **v0.dev (Vercel IA)**: [https://v0.dev](https://v0.dev)

### Integrações & APIs
* **Uazapi (Documentação)**: [https://docs.uazapi.com](https://docs.uazapi.com)
* **Meta for Developers (WhatsApp)**: [https://developers.facebook.com/docs/whatsapp](https://developers.facebook.com/docs/whatsapp)

### Infraestrutura & Gestão
* **GitHub**: [https://github.com](https://github.com)
* **Vercel**: [https://vercel.com/docs](https://vercel.com/docs)
* **Railway**: [https://docs.railway.app](https://docs.railway.app)
* **Postman**: [https://learning.postman.com](https://learning.postman.com)

## 6. Apêndices (Opcionais)

Informações complementares, dados de suporte ou discussões detalhadas fora do corpo principal.

## 7. Avaliações de Professores

Adicionar três páginas no final do RFC para que os Professores escolhidos possam fazer suas considerações e assinatura:
- Considerações Professor/a:
- Considerações Professor/a:
- Considerações Professor/a:
