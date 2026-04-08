---
name: linkedin-feed-publisher
description: Estruture, otimize e implemente a publicacao no feed do LinkedIn a partir de telas, slides ou cards de produto. Use quando for criar a action de compartilhar no LinkedIn, gerar copy a partir do conteudo visivel de um slide, montar payloads de compartilhamento, definir UX de share ou transformar uma ideia, anuncio, case ou resumo visual em um post claro, escaneavel e publicavel.
---

# LinkedIn Feed Publisher

Use esta skill para transformar o conteudo de uma tela ou slide em uma action de compartilhamento no LinkedIn com copy pronta.

## Regras Base

Sempre:
- parta do conteudo do slide atual
- abra com um hook forte nas 1 a 3 primeiras linhas
- escreva para leitura rapida em feed
- use paragrafos curtos e espacados
- mantenha tom humano, especifico e profissional
- evite tom generico de IA, hype vazio e jargoes em excesso
- preserve substancia: opiniao, dado, aprendizado ou narrativa concreta
- termine com CTA quando isso ajudar o objetivo da publicacao

## Fluxo

1. Identifique o objetivo do post: alcance, autoridade, anuncio, contratacao, engajamento ou narrativa pessoal.
2. Identifique a origem: slide unico, tela de resumo, card de metrica ou retrospectivo completo.
3. Identifique o formato: texto curto, texto medio, texto longo, carrossel ou comentario de apoio.
4. Extraia o nucleo: problema, insight, prova, resultado ou opiniao.
5. Construa na ordem: hook > contexto > desenvolvimento > fechamento > CTA.
6. Se o pedido for de implementacao, defina a action de share, o texto base e o comportamento de fallback.

## Formato Preferido

Quando gerar copy, entregue:
- objetivo
- origem do conteudo
- publico-alvo
- versao principal
- 3 hooks alternativos, se houver espaco
- CTA sugerido
- hashtags apenas se forem realmente uteis

Quando o pedido for de implementacao, entregue:
- ponto de entrada do botao
- regra para montar a copy a partir do slide
- payload ou URL de compartilhamento
- estados de UX
- fallback quando nao houver imagem, link ou contexto suficiente

## Referencias

Leia so o necessario:
- `references/post-playbooks.md` para estruturas de post por objetivo
- `references/style-guards.md` para tom, clareza e anti-padroes
- `references/share-action.md` para implementar botao, fluxo e payload de compartilhamento

## Guardrails

Nao:
- gere copy desconectada do slide atual
- use abertura morna
- escreva blocos longos e densos
- use emojis em excesso
- use hashtags demais
- prometa o que o conteudo nao entrega
- force vulnerabilidade ou storytelling artificial

Faca:
- priorize clareza, ritmo e especificidade
- adapte o post ao objetivo real
- preserve o contexto do slide na copy compartilhada
- preserve a voz do autor sempre que houver insumo
