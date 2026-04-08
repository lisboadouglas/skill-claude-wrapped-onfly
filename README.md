# Onfly Retrospective Design Skill

Skill para orientar o Claude Code na criação de experiências retrospectivas da Onfly para viagens e despesas corporativas.

## O que esta skill cobre

- `Wrapped Onfly`: retrospectiva anual com narrativa mais forte e foco em apresentação.
- `Capsula de Viagens`: retrospectiva mensal, mais leve e recorrente.
- Perfil `gestor`: visão consolidada da empresa.
- Perfil `colaborador`: visão individual.
- Modo extra: gestor visualizando os `wrappeds` e `capsulas` individuais do time.

## Objetivo

Transformar dados de viagens e despesas corporativas em experiências visuais, narrativas e acionáveis, com uma camada de IA para interpretar comportamento, destacar padrões e sugerir próximas ações.

## Estrutura

```text
skills/onfly-retrospective-design/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── evaluation-criteria.md
    ├── implementation-prompts.md
    ├── mock-data-schema.md
    └── screen-playbooks.md
```

## Como usar

Exemplo de invocação:

```text
Use $onfly-retrospective-design para definir telas, narrativa e insights com IA para o Wrapped Onfly ou para a Capsula de Viagens.
```

## Arquivos principais

- `SKILL.md`: regras centrais, fluxo, tom, padroes de IA e guardrails.
- `references/screen-playbooks.md`: roteiro de telas por produto e perfil (fonte canonica).
- `references/evaluation-criteria.md`: criterios de avaliacao para pitch e proposta de valor.
- `references/mock-data-schema.md`: schema de dados mockados para consistencia entre telas.
- `references/implementation-prompts.md`: prompts prontos para o usuario invocar a skill.
- `claude-master-prompt.md`: prompt enxuto que invoca a skill e complementa com specs de arquitetura, UX e entrega.

## Casos de uso

- Definir conceito de produto para demo ou hackathon.
- Gerar roteiro de telas por perfil.
- Produzir copy inicial para a experiência.
- Criar prompts de implementação para Claude Code.
- Guiar a construção de uma interface demo com mocks.

## Princípios da skill

- Separar claramente `gestor` e `colaborador`.
- Tratar a visão do gestor sobre o time como acompanhamento e reconhecimento, não fiscalização.
- Usar IA como camada de interpretação e recomendação, não como buzzword.
- Manter a proposta implementável e pronta para pitch.
- Economizar tokens, deixando o `SKILL.md` enxuto e os detalhes em referências específicas.

## Status

- Skill criada e validada.
- Prompt mestre criado para implementação completa.
