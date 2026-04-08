---
name: onfly-retrospective-design
description: Estruture e especifique experiencias retrospectivas da Onfly para usuarios de viagens e despesas corporativas. Use quando for definir estrategia de produto, fluxos de UX, conceitos de telas, copy, insights com IA ou pitch para o Wrapped Onfly (retrospectiva anual) e para a Capsula de Viagens (retrospectiva mensal), especialmente quando a experiencia precisar suportar gestor, colaborador e a visao do gestor sobre os retrospectivos individuais do time.
---

# Onfly Retrospective Design

Use esta skill para definir rapidamente:
- `Wrapped Onfly`: retrospectiva anual
- `Capsula de Viagens`: retrospectiva mensal
- perfis `gestor` e `colaborador`
- modo extra: gestor vendo retrospectivos individuais do time

## Regras Base

Sempre:
- trate isso como produto de travel tech B2B, nao como relatorio bonito
- separe `gestor` e `colaborador` como narrativas distintas
- trate a visao do gestor sobre o time como acompanhamento e reconhecimento, nao fiscalizacao
- use IA para interpretar, resumir e recomendar; nao apenas decorar a interface
- mantenha o escopo MVP e pitchavel
- detecte a stack tecnica do projeto alvo (framework, linguagem, CSS) antes de implementar; nao assuma React ou qualquer stack fixa
- mapas e rotas sao visuais mockados (SVG ou imagem estatica), nao integracoes com Mapbox/Leaflet

## Fluxo

Siga esta ordem:
1. Identifique a entrega: pitch, telas, copy, PRD ou prompt de implementacao.
2. Escolha o produto: `Wrapped Onfly` ou `Capsula de Viagens`.
3. Escolha o perfil: `gestor`, `colaborador` ou `gestor visualizando o time`.
4. Monte a sequencia: abertura > numeros > interpretacao > recomendacao > fechamento.
5. Inclua um momento explicito de IA.
6. Feche com valor de negocio.

## Formato Preferido

Quando o pedido for de telas, responda por tela com:
- nome
- objetivo
- dado ou insight principal
- ideia visual
- CTA ou continuidade

Quando o pedido for de implementacao, entregue:
- estrutura de pagina
- componentes
- dados mockados necessarios
- comportamento responsivo
- direcao visual

## Tom

Evite tom frio de dashboard de BI e linguagem de entretenimento copiada do Spotify.
Busque: premium, claro, energico, util, corporativo sem soar burocratico.

## Padroes de IA

Use IA para produzir:
- resumo executivo em um paragrafo
- resumo pessoal em um paragrafo
- headlines de anomalia
- bullets de recomendacao
- rotulos comportamentais como `planejador eficiente` ou `operacao sob pressao`
- leitura resumida do perfil de viagem de cada colaborador para o gestor

Mantenha a linguagem especifica, nao mistica.

## Referencias

Leia so o necessario:
- `references/screen-playbooks.md` para roteiros de telas por produto e perfil
- `references/evaluation-criteria.md` para ajustar pitch e proposta de valor
- `references/mock-data-schema.md` para estrutura de dados mockados

## Guardrails

Nao:
- reduza os dois perfis a um unico dashboard generico
- trate a visao do gestor sobre o time como vigilancia sem contexto ou sensibilidade
- dependa apenas de metricas vaidosas sem interpretacao
- use IA como buzzword sem valor visivel para o usuario
- faca a capsula mensal parecer uma copia mais fraca do wrapped anual

Faca:
- cada produto ter cadencia e intencao proprias
- a camada de supervisao do gestor reforcar desenvolvimento do time, reconhecimento e tomada de decisao
- o contexto de travel tech aparecer de forma clara
- a resposta ser concisa, apresentavel e pronta para implementacao
