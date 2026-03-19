# Prompt 04 — UI/UX
## Criar telas e componentes descrevendo em texto

**Quando usar:** Para construir qualquer tela ou componente do sistema.

---

## Prompt (copie e cole no Claude Code)

```
Preciso criar a tela de [NOME DA TELA, ex: dashboard principal / listagem de leads / cadastro de produto].

O que essa tela precisa mostrar/fazer:
- [ex: cards com métricas no topo: total de leads, leads hoje, taxa de conversão]
- [ex: tabela com todos os leads, com filtro por status e busca por nome]
- [ex: botão para cadastrar novo lead que abre um modal com formulário]
- [adicione o que precisar]

Nossa stack de UI:
- Next.js com App Router (use componentes no padrão /app)
- Tremor para gráficos, cards de métricas e tabelas de dados
- Origin UI para formulários, modais, botões e inputs
- Cosmos UI para componentes de layout e navegação
- Tailwind CSS para estilos customizados
- Use o padrão do skill ui-ux-pro-max para estrutura visual

Estilo visual:
- [ex: dark mode / claro / siga o padrão já existente no projeto]
- [ex: paleta de cores principal: azul corporativo / laranja / roxo]

Com base nisso:
1. Crie o componente da tela completo e funcional
2. Use dados mockados por enquanto (vou conectar ao backend depois)
3. A tela deve funcionar bem no mobile e no desktop
4. Separe em subcomponentes se a tela for complexa
```

---

## Dicas

- Descreva a tela como se estivesse explicando para um designer — seja visual
- "Dados mockados" significa que o Claude vai criar dados falsos para você ver como fica
- Depois que aprovar o visual, use o Prompt 05 (Integração) para conectar à API real
