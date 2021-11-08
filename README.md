# Gestão e Esquema Inteligente para Banco de Dados
Sugestão/esquema para usar um banco de dados open-source considerando uma alta disponibilidade, desempenho, disponibilidade, redundância, e também um baixo custo.

### 1 - Supabase (PostgreSQL):
Seria o núcleo geral do armazenamento em nuvem e escalável de todas as informações/dados gerenciados pela aplicação
(https://supabase.io/)

### 2 - Upstash (Redis):
Iria servir informações onde os acessos são mais constantes/frequentes ou críticos
(https://upstash.com/)

### 3 - Local Storage:
Iria usar o armazenamento do browser para servir/exibir informações não-sensíveis, preferências do usuário, etc...
(https://developer.mozilla.org/pt-BR/docs/Web/API/Window/localStorage)
