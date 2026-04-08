# Onfly Skills

Repositorio de skills para o Claude Code orientar a criacao de produtos e conteudo da Onfly.

## Skills disponiveis

### 1. `onfly-retrospective-design`

Experiencias retrospectivas de viagens e despesas corporativas.

**Produtos**: Wrapped Onfly (anual) e Capsula de Viagens (mensal).
**Perfis**: gestor (consolidado), colaborador (individual), gestor vendo colaborador.

```text
Use $onfly-retrospective-design para definir telas, narrativa e insights com IA para o Wrapped Onfly ou para a Capsula de Viagens.
```

Estrutura:
```text
skills/onfly-retrospective-design/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── evaluation-criteria.md
    ├── implementation-prompts.md  (menu de prompts para o usuario)
    ├── mock-data-schema.md
    └── screen-playbooks.md
```

Arquivos-chave:
- `SKILL.md`: regras, fluxo, tom, padroes de IA e guardrails.
- `references/screen-playbooks.md`: roteiro de telas por produto e perfil (fonte canonica).
- `references/mock-data-schema.md`: schema de dados mockados para consistencia.
- `references/evaluation-criteria.md`: criterios de avaliacao para pitch.
- `claude-master-prompt.md`: prompt enxuto que invoca a skill com specs de arquitetura, UX e entrega.

---

### 2. `linkedin-feed-publisher`

Transforma conteudo de telas, slides ou cards em posts e actions de compartilhamento no LinkedIn.

**Modos**: gerar copy de post ou implementar botao de share no frontend.

```text
Use $linkedin-feed-publisher para criar copy ou implementar a action de compartilhar no LinkedIn a partir de um slide ou tela.
```

Estrutura:
```text
skills/linkedin-feed-publisher/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── post-playbooks.md
    ├── style-guards.md
    └── share-action.md
```

Arquivos-chave:
- `SKILL.md`: regras de escrita para feed, fluxo, formato de entrega e guardrails.
- `references/post-playbooks.md`: estruturas de post por objetivo (lancamento, case, aprendizado, bastidor, contratacao).
- `references/style-guards.md`: tom, clareza, hooks, anti-padroes e regras de hashtag.
- `references/share-action.md`: implementacao do botao de share (UX, payload, estados, fallbacks).

---

## Principios gerais

- Cada skill detecta a stack tecnica do projeto alvo antes de implementar.
- `SKILL.md` funciona como indice enxuto; detalhes vivem nas references.
- Economizar tokens: ler so o necessario por tarefa.
