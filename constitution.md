Diretrizes e Arquitetura do Projeto

1. Stack Tecnológica (Strict Client-Side)
* **Frontend:** HTML5 semântico e CSS3 estruturado via Grid/Flexbox.
* **Lógica:** Vanilla JavaScript (ES6+) sem frameworks externos.
* **Persistência:** Web Storage API (`localStorage`) para retenção de dados entre sessões.
* **Criptografia/Codificação:** Utilização da API nativa `btoa()` e `atob()` (Base64) para portabilidade de dados.

2. Princípios de UI/UX (Design System)
* **Tema Dark:** Fundo `#0f111a` com superfícies em `#1e212b`.
* **Cores de Destaque:** Neutros em `#f1f2f6`, destaques em `#00ffcc` (Neon Cyan) e estados críticos em `#ff4757`.
* **Acessibilidade Visivel:** Mudanças de estado instantâneas (ex: barra de orçamento mudando para vermelho) para feedbacks de erro.

3. Regras de Código e Resiliência
* Todo ID gerado para novos componentes deve utilizar `crypto.randomUUID()`.
* Chamadas assíncronas (`fetch`) devem obrigatoriamente possuir blocos `try/catch` com uma base de dados *fallback* local estática em memória para garantir operação offline.