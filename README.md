# Gestão e Esquema Inteligente para Banco de Dados
Sugestão/esquema para usar um banco de dados open-source considerando uma alta disponibilidade, desempenho, redundância e também baixo custo.

### 1 - Supabase (PostgreSQL):
Seria o "núcleo geral" do armazenamento em nuvem de todas as informações/dados gerenciados pela aplicação e consumidos pelos usuários da aplicação. Resumindo: seria o banco de dados principal.
(https://supabase.io/)

### 2 - Upstash (Redis):
Iria servir informações onde os acessos são mais constantes/frequentes ou críticos
(https://upstash.com/)

### 3 - Local Storage:
Iria usar o armazenamento do browser para servir/exibir informações não-sensíveis, preferências do usuário, etc...
(https://developer.mozilla.org/pt-BR/docs/Web/API/Window/localStorage)

Todas as tecnologias citadas podem ser usadas de forma integrada, bem planejada e estruturada. Isso iria trazer ótimos benefícos referente a desempenho e redução de custo com provedores como Amazon AWS, Google Cloud, Azure, etc...

Tudo isso que falei é um setup exclusivo para **banco de dados** (tratamento de todos os dados da aplicação e de usuários que consomem a aplicação). Ou seja, nada relacionado a linguagens/tecnologias server-side rodando em containers orquestrados. E também nada relacionado a front-end e/ou arquivos estáticos (css, js, img...). A respeito desses 2 (linguagens server-side e front-end) irei abordar em outro repositório em breve.
