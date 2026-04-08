# Claude Master Prompt

```text
Use $onfly-retrospective-design.

Implemente de uma vez a interface completa dos dois produtos da Onfly:
1. Wrapped Onfly
2. Capsula de Viagens

A experiencia deve suportar 3 modos de visualizacao:
1. gestor com visao consolidada da empresa
2. colaborador com visao individual
3. gestor visualizando os retrospectivos individuais dos colaboradores do time

Siga os roteiros de tela em references/screen-playbooks.md.
Siga os criterios de valor em references/evaluation-criteria.md.
Use a estrutura de mocks em references/mock-data-schema.md.

Arquitetura:
- detecte a stack do projeto antes de implementar
- layout principal + paginas/secoes + componentes reutilizaveis
- home inicial para escolher produto e perfil
- navegacao clara entre fluxos e modos
- componentes reutilizaveis: hero de abertura, cards de metricas, mapas/rotas mockados, timeline/barras, resumo de IA, cards de colaborador, blocos de recomendacao

Dados mockados:
- siga o schema em references/mock-data-schema.md
- 1 gestor + 4 colaboradores
- consistencia entre visao consolidada e visoes individuais

UX:
- gestor deve saber se esta vendo empresa, time ou individuo
- colaborador deve parecer pessoal, nao recorte menor do gestor
- CTAs claros para avancar na narrativa
- troca entre Wrapped e Capsula simples

Entrega:
- interface completa funcionando com mocks, sem backend
- responsivo mobile + desktop
- textos e headlines prontos
- ao final: resuma o criado, liste componentes, diga o que falta para producao

Economize tokens: nao explique, implemente.
```
