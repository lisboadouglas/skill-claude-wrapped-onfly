# Share Action

Use este guia quando a task for implementar o botao de compartilhar no LinkedIn a partir de um slide.

## Objetivo

Permitir que cada slide gere uma copy curta, coerente e compartilhavel no feed do LinkedIn sem exigir edicao manual obrigatoria.

## Fluxo recomendado

1. Usuario clica em `Compartilhar no LinkedIn`
2. Sistema le o contexto do slide atual
3. Sistema monta uma copy base otimizada
4. Usuario pode:
- publicar direto via URL de compartilhamento, quando aplicavel
- copiar a copy
- baixar ou anexar imagem do slide, se existir

## O que extrair do slide

- titulo
- subtitulo
- metrica principal
- insight principal
- contexto do perfil ou produto

## Formula curta de copy

1. Hook derivado do insight
2. 1 ou 2 linhas de contexto
3. 1 linha de fechamento ou CTA

## Exemplo de payload logico

- `title`: titulo do slide
- `summary`: insight principal
- `shareText`: copy final para feed
- `shareUrl`: link publico, se existir
- `imageUrl`: imagem do slide, se existir

## Estados de UX

- botao padrao
- gerando copy
- copy pronta
- copiar texto
- abrir LinkedIn
- erro com fallback para copiar texto

## Guardrails

- nao dependa de integracao complexa para o MVP
- priorize `copiar texto + abrir LinkedIn`
- trate imagem do slide como opcional
- mantenha a copy curta o suficiente para compartilhar sem edicao pesada
