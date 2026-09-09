# Prompt 02 — BANCO
## Criar tabelas, relações e migrações no PostgreSQL

**Quando usar:** Sempre que precisar criar ou alterar a estrutura do banco de dados.

---

## Prompt para o Codex

```
Preciso criar as tabelas do banco de dados para o sistema [NOME DO SISTEMA].

O que o sistema precisa armazenar:
- [ex: usuários com nome, email, senha e nível de acesso]
- [ex: leads com nome, telefone, status e responsável]
- [ex: tarefas com título, descrição, prazo e status]
- [adicione o que precisar]

Relações entre as tabelas:
- [ex: cada lead pertence a um usuário responsável]
- [ex: cada tarefa pode ter vários comentários]

Nosso banco é PostgreSQL rodando no Coolify. Usamos o pacote `pg` (node-postgres) para conectar — sem ORM.

Com base nisso:
1. Crie as tabelas com todos os campos necessários, tipos corretos e constraints
2. Crie as chaves estrangeiras para as relações descritas
3. Crie os índices nos campos que vão ser mais pesquisados
4. Gere o arquivo SQL com todas as queries de criação (migration)
5. Crie um arquivo `db.js` no backend com a conexão configurada usando variável de ambiente DATABASE_URL
6. Crie uma função de seed com dados de exemplo para eu testar
```

---

## Dicas

- Sempre descreva as relações claramente — isso evita retrabalho depois
- O arquivo SQL gerado pode ser rodado direto no painel do PostgreSQL no Coolify
- Se precisar alterar uma tabela depois, use este prompt novamente descrevendo só a alteração
