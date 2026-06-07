# Smart Stock - Frontend

## Descrição do Projeto

O Smart Stock é uma aplicação frontend desenvolvida para gerenciar o estoque de medicamentos, com foco em farmácias. Ele oferece um painel de controle intuitivo para visualização rápida do inventário, funcionalidades de login e logout, registro de entradas e saídas de produtos, e um sistema de alertas para estoque crítico e medicamentos próximos ao vencimento. A aplicação interage com uma API backend para persistência e recuperação de dados.

## Funcionalidades

- **Autenticação de Usuário**: Sistema de login seguro com validação de credenciais via API e gerenciamento de sessão.
- **Dashboard Interativo**: Visão geral do estoque com indicadores de total de itens, estoque crítico e volume geral.
- **Alertas e Notificações**: Notificações em tempo real para medicamentos com estoque baixo ou próximos ao vencimento.
- **Registro de Movimentações**: Modais dedicados para lançamento de entradas e saídas de medicamentos do estoque.
- **Navegação Simples**: Menu lateral para acesso rápido a diferentes seções da aplicação (Dashboard, Cadastro de Medicamentos, Histórico de Movimentações, Relatórios).
- **Design Responsivo**: Interface de usuário moderna e adaptável, construída com CSS puro e variáveis.

## Tecnologias Utilizadas

- **HTML5**: Estrutura semântica das páginas.
- **CSS3**: Estilização completa da aplicação, utilizando variáveis CSS para facilitar a manutenção e customização.
- **JavaScript (ES6+)**: Lógica de frontend, interações com o usuário e comunicação com a API.
- **Local Storage**: Armazenamento de token de autenticação e dados do usuário para gerenciamento de sessão.
- **Fetch API**: Para realizar requisições HTTP assíncronas ao backend.
