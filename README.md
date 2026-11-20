# MovieFlow: 13 modelos

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


[![MovieFlow: 13 modelos](guia/assets/banner.jpg)](https://inematds.github.io/movieflow-modelos/guia/)

**ðŸ‡§ðŸ‡· [PortuguÃªs](README.md) Â· ðŸ‡ºðŸ‡¸ [English](README.en.md) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](README.es.md)**

## O que Ã©

O MovieFlow (movieflow.ai) Ã© um estÃºdio de filmes com IA: vocÃª escreve uma ideia e ele monta a histÃ³ria, os personagens, as cenas e o filme. Por trÃ¡s dele hÃ¡ 13 modelos de outras empresas (Seedance, Kling, Veo, MiniMax, Vidu, Nano Banana, GPT Image e outros), e cada um Ã© melhor numa coisa. Este projeto reÃºne, num guia e num arquivo de dados, o que cada modelo faz, os limites e quando usar. Para usar Ã© sÃ³ ler a pÃ¡gina; quem quiser pode rodar o escolhedor no terminal com Python, sem instalar nada.

## ðŸŽ¬ VÃ­deo

https://www.youtube.com/watch?v=0zyz-H-1qXQ (16:9) Â· short: https://www.youtube.com/watch?v=WizdRuVKl1U

## ðŸ“– Guia de uso

Guia completo (landing + passo a passo): **https://inematds.github.io/movieflow-modelos/guia/**

## Os 13 modelos

| Modelo | Tipo | Use quando |
|---|---|---|
| Seedance 2.5 | vÃ­deo | plano longo (atÃ© 30 s) com som e o mesmo personagem |
| MovieFlow 2.0 Ultra | vÃ­deo | rascunho rÃ¡pido e barato (US$ 0,008/s) |
| MiniMax H3 | vÃ­deo | imagem 2K nÃ­tida, referÃªncias, corrigir um detalhe |
| Kling 3.0 | vÃ­deo | cortes (2 a 6 planos), aÃ§Ã£o, fala sincronizada |
| Seedance 2.0 | vÃ­deo | copiar movimento/estilo de uma referÃªncia |
| Vidu Q3 Pro | vÃ­deo | conversa entre vÃ¡rios personagens, anime |
| Veo 3 | vÃ­deo | plano curto realista com fala e ambiente |
| Seedance Fast | vÃ­deo | testar vÃ¡rias versÃµes barato (atÃ© 720p) |
| Kling 2.6 | vÃ­deo | cena simples de 5â€“10 s, copiar gesto |
| Nano Banana Pro | imagem | texto na imagem, quadro-chave do personagem |
| Nano Banana 2 | imagem | muitas imagens rÃ¡pidas (storyboard) |
| GPT Image 2 | imagem | texto denso, diagrama, painel de HQ, retoque |
| Seedream 5.0 | imagem | 4K barato, editar sÃ³ uma regiÃ£o |

Fontes e limites de cada um em `modelos.json` (dados de 06/11/2026; "diverge" = fontes nÃ£o batem).

## O processo, do inÃ­cio ao fim

1. ðŸ§  **Escolher o modelo da cena** â€” `python3 escolher.py "descriÃ§Ã£o da cena"` (ou os botÃµes do guia).
2. ðŸ§  **Ver a ficha** â€” `python3 escolher.py --modelo kling-3.0` / `--lista --tipo video`.
3. ðŸ§  **Criar no MovieFlow** â€” movieflow.ai â†’ Agent V2 â†’ ideia, idioma, duraÃ§Ã£o, formato â†’ Create; rascunho no modelo barato, cena final no indicado.
4. ðŸ§  **Atualizar os dados** quando a lista do MovieFlow mudar â€” editar `modelos.json`.
5. âš™ï¸ **Remontar a pÃ¡gina** â€” `python3 montar_guia.py` (gera `guia/index.html`); ðŸ¤– retraduzir `guia/en/` e `guia/es/`.
6. âš™ï¸ **Publicar** â€” commit + push; o GitHub Pages (Actions) publica sozinho.

Legenda: ðŸ§  sessÃ£o com o Nei Â· âš™ï¸ script Â· ðŸ¤– agente.

## Arquivos

- `modelos.json` â€” os 13 modelos (fabricante, duraÃ§Ã£o, Ã¡udio, destaque, use quando, limites, fontes).
- `escolher.py` â€” indica o modelo pela descriÃ§Ã£o da cena (Python 3, sem dependÃªncias, sem rede).
- `montar_guia.py` â€” monta `guia/index.html` a partir do `modelos.json`.
- `guia/` â€” pÃ¡gina em PT, `guia/en/` e `guia/es/`.

LicenÃ§a MIT Â· [INEMA.CLUB](https://inema.club)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>