# Prompt 01 — ARQUITETURA
## Iniciar qualquer projeto do zero sem travar

**Quando usar:** No primeiro dia de um novo projeto, antes de escrever qualquer código.

---

## Prompt para o Codex

```
Vou construir um sistema chamado [NOME DO SISTEMA].

O que ele precisa fazer:
- [descreva a função principal, ex: gerenciar leads de vendas]
- [descreva a segunda função, ex: enviar mensagens via WhatsApp]
- [adicione quantas funções precisar]

Quem vai usar: [ex: time de vendas interno / clientes finais / apenas eu]

Nossa stack é:
- Frontend: Next.js com App Router, deploy na Vercel
- Backend: Node.js com Express, deploy no Coolify (Hostinger)
- Banco: PostgreSQL rodando no Coolify
- Auth: JWT (não use Supabase Auth)
- UI: Tremor, Origin UI e Cosmos UI

Com base nisso:
1. Crie a estrutura completa de pastas do projeto (frontend e backend separados)
2. Inicialize o projeto com os pacotes essenciais já instalados
3. Crie um arquivo AGENTS.md na raiz explicando a arquitetura para as próximas sessões
4. Crie um arquivo .env.example com todas as variáveis que vou precisar configurar
5. Me mostre o próximo passo depois de tudo criado
```

---

## Dicas

- Seja específico na descrição do sistema — quanto mais detalhes, melhor a estrutura gerada
- O `AGENTS.md` gerado vai ser a memória do projeto para sessões futuras
- Depois que rodar, verifique o `.env.example` e crie seu `.env` com os valores reais
