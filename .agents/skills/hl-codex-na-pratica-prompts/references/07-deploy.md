# Prompt 07 — DEPLOY
## Colocar o sistema no ar com domínio e HTTPS

**Quando usar:** Para fazer o primeiro deploy ou atualizar o sistema em produção.

---

## Prompt — Primeiro deploy (copie e cole no Codex)

```
Preciso colocar o sistema [NOME DO SISTEMA] no ar pela primeira vez.

Estrutura do projeto:
- Frontend: Next.js em /frontend → vai para a Vercel
- Backend: Node.js com Express em /backend → vai para o Coolify (Hostinger)
- Banco: PostgreSQL já está rodando no Coolify

Domínio:
- Frontend: [ex: meusistema.com.br / app.meusistema.com.br]
- Backend/API: [ex: api.meusistema.com.br]

Por favor:
1. Verifique se o projeto está pronto para deploy (checklist de produção)
2. Crie o arquivo vercel.json se necessário para o frontend
3. Crie o Dockerfile para o backend rodar no Coolify
4. Liste todas as variáveis de ambiente que preciso configurar na Vercel e no Coolify
5. Me dê o passo a passo para conectar o domínio na Vercel e no Coolify
6. Me diga como confirmar que tudo está funcionando em produção
```

---

## Prompt — Atualizar o sistema já em produção

```
Preciso atualizar o sistema em produção com as mudanças que fiz.

O que mudei:
- [ex: adicionei uma nova tela de relatórios]
- [ex: corrigi o bug no formulário de cadastro]
- [ex: adicionei uma nova coluna na tabela de leads]

Tem mudança no banco de dados? [sim / não]
Se sim, descreva: [ex: adicionei o campo "origem" na tabela leads]

Por favor:
1. Se tiver mudança no banco, gere o SQL de alteração para rodar antes do deploy
2. Verifique se tem algum problema que pode quebrar a produção
3. Me dê a sequência correta para atualizar sem derrubar o sistema
```

---

## Dicas

- Nunca atualize o banco de produção sem fazer backup antes — peça ao Codex como fazer
- Variáveis de ambiente de produção NUNCA devem ser as mesmas do desenvolvimento
- Se o deploy falhar no Coolify, vá em Logs do deployment e cole o erro aqui
