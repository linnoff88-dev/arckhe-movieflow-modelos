ï»¿# MovieFlow: 13 modelos

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


[![MovieFlow: 13 modelos](guia/assets/banner.jpg)](https://linnoff88-dev.github.io/arckhe-/guia/)

**ê°Å¸â¡Â§ê°Å¸â¡Â· [PortuguêÂªs](README.md) êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](README.en.md) êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](README.es.md)**

## O que êÂ©

O MovieFlow (movieflow.ai) êÂ© um estêÂºdio de filmes com IA: vocêÂª escreve uma ideia e ele monta a histêÂ³ria, os personagens, as cenas e o filme. Por trêÂ¡s dele hêÂ¡ 13 modelos de outras empresas (Seedance, Kling, Veo, MiniMax, Vidu, Nano Banana, GPT Image e outros), e cada um êÂ© melhor numa coisa. Este projeto reêÂºne, num guia e num arquivo de dados, o que cada modelo faz, os limites e quando usar. Para usar êÂ© sêÂ³ ler a pêÂ¡gina; quem quiser pode rodar o escolhedor no terminal com Python, sem instalar nada.

## ê°Å¸Å½Â¬ VêÂ­deo

https://www.youtube.com/watch?v=0zyz-H-1qXQ (16:9) êÂ· short: https://www.youtube.com/watch?v=WizdRuVKl1U

## ê°Å¸ââ Guia de uso

Guia completo (landing + passo a passo): **https://linnoff88-dev.github.io/arckhe-/guia/**

## Os 13 modelos

| Modelo | Tipo | Use quando |
|---|---|---|
| Seedance 2.5 | vêÂ­deo | plano longo (atêÂ© 30 s) com som e o mesmo personagem |
| MovieFlow 2.0 Ultra | vêÂ­deo | rascunho rêÂ¡pido e barato (US$ 0,008/s) |
| MiniMax H3 | vêÂ­deo | imagem 2K nêÂ­tida, referêÂªncias, corrigir um detalhe |
| Kling 3.0 | vêÂ­deo | cortes (2 a 6 planos), aêÂ§êÂ£o, fala sincronizada |
| Seedance 2.0 | vêÂ­deo | copiar movimento/estilo de uma referêÂªncia |
| Vidu Q3 Pro | vêÂ­deo | conversa entre vêÂ¡rios personagens, anime |
| Veo 3 | vêÂ­deo | plano curto realista com fala e ambiente |
| Seedance Fast | vêÂ­deo | testar vêÂ¡rias versêÂµes barato (atêÂ© 720p) |
| Kling 2.6 | vêÂ­deo | cena simples de 5ê¢â¬â10 s, copiar gesto |
| Nano Banana Pro | imagem | texto na imagem, quadro-chave do personagem |
| Nano Banana 2 | imagem | muitas imagens rêÂ¡pidas (storyboard) |
| GPT Image 2 | imagem | texto denso, diagrama, painel de HQ, retoque |
| Seedream 5.0 | imagem | 4K barato, editar sêÂ³ uma regiêÂ£o |

Fontes e limites de cada um em `modelos.json` (dados de 06/11/2026; "diverge" = fontes nêÂ£o batem).

## O processo, do inêÂ­cio ao fim

1. ê°Å¸Â§Â  **Escolher o modelo da cena** ê¢â¬â `python3 escolher.py "descriêÂ§êÂ£o da cena"` (ou os botêÂµes do guia).
2. ê°Å¸Â§Â  **Ver a ficha** ê¢â¬â `python3 escolher.py --modelo kling-3.0` / `--lista --tipo video`.
3. ê°Å¸Â§Â  **Criar no MovieFlow** ê¢â¬â movieflow.ai ê¢â â Agent V2 ê¢â â ideia, idioma, duraêÂ§êÂ£o, formato ê¢â â Create; rascunho no modelo barato, cena final no indicado.
4. ê°Å¸Â§Â  **Atualizar os dados** quando a lista do MovieFlow mudar ê¢â¬â editar `modelos.json`.
5. ê¢Å¡â¢ê¯Â¸Â **Remontar a pêÂ¡gina** ê¢â¬â `python3 montar_guia.py` (gera `guia/index.html`); ê°Å¸Â¤â retraduzir `guia/en/` e `guia/es/`.
6. ê¢Å¡â¢ê¯Â¸Â **Publicar** ê¢â¬â commit + push; o GitHub Pages (Actions) publica sozinho.

Legenda: ê°Å¸Â§Â  sessêÂ£o com o Nei êÂ· ê¢Å¡â¢ê¯Â¸Â script êÂ· ê°Å¸Â¤â agente.

## Arquivos

- `modelos.json` ê¢â¬â os 13 modelos (fabricante, duraêÂ§êÂ£o, êÂ¡udio, destaque, use quando, limites, fontes).
- `escolher.py` ê¢â¬â indica o modelo pela descriêÂ§êÂ£o da cena (Python 3, sem dependêÂªncias, sem rede).
- `montar_guia.py` ê¢â¬â monta `guia/index.html` a partir do `modelos.json`.
- `guia/` ê¢â¬â pêÂ¡gina em PT, `guia/en/` e `guia/es/`.

LicenêÂ§a MIT êÂ· [ARCKHÉ AI](https://ARCKHÉ AI)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>