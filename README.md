# Agentes não fogem — slides

**Slides online:** https://sschonss.github.io/talk-agents-dont-escape/
**PDF:** https://sschonss.github.io/talk-agents-dont-escape/agents-dont-escape.pdf

Deck em [Marp](https://marp.app) baseado no artigo
[Agentes não fogem: a gente deixa a porta aberta](https://luizschons.com/pt-br/posts/agents-dont-escape/)
e no lab [agent-containment-lab](https://github.com/sschonss/agent-containment-lab).
É a continuação da palestra [Design for Failure](https://luizschons.com/pt-br/posts/design-for-failure/).

- `slides.md`: o deck (44 slides, ~40 min, só slides). A Parte 4 mostra, porta a porta, as saídas reais do lab (`docs/RESULTS.md`). Os slides têm pouco texto. O roteiro e as fontes ficam nas **notas do apresentador** (`<!-- ... -->`).
- `themes/aifa.css`: o mesmo tema da talk AI-Friendly Architecture, mais blocos de terminal e placeholders.
- `assets/`: foto, diagrama do lab e QR codes.

O deploy no GitHub Pages roda a cada push na `main` (`.github/workflows/pages.yml`).

## Comandos

```bash
npm run dev     # servidor com preview ao vivo
npm run build   # dist/index.html (modo apresentador: tecla P)
npm run pdf     # dist/agents-dont-escape.pdf
npm run pptx    # dist/agents-dont-escape.pptx
```

Sem instalar nada:

```bash
npx -y @marp-team/marp-cli@4.2.3 --no-stdin slides.md --allow-local-files -o dist/index.html
```

## Pendências antes do evento

- [ ] QR de feedback: gerar com os ids do Sessionize (`/pt-br/feedback/?t=<id>&e=<id>`) e trocar o placeholder do último slide.
