# Schema de Dados Mockados

Use esta estrutura para garantir consistencia entre telas e perfis. Popule com valores plausiveis de travel tech corporativa brasileira.

## Empresa

```
company:
  name: string           # ex: "TechNova Ltda"
  sector: string         # ex: "Tecnologia"
  employees_count: number
  cost_centers: string[] # ex: ["Engenharia", "Comercial", "Produto"]
  policy_compliance_rate: number # percentual
  year: number           # ano do wrapped
  month: string          # mes da capsula
```

## Gestor

```
manager:
  name: string
  role: string           # ex: "Head de Operacoes"
  department: string
  team_size: number
```

## Colaboradores (minimo 4)

```
employee:
  name: string
  role: string
  department: string
  cost_center: string
  traveler_label: string  # ex: "planejador eficiente", "viajante de ultima hora"
  compliance_score: number
```

## Viagens

```
trip:
  employee_id: string
  origin: string         # cidade
  destination: string    # cidade
  date: date
  return_date: date
  advance_days: number   # dias de antecedencia da reserva
  booking_type: string   # "self-booking" | "solicitacao" | "emergencial"
  in_policy: boolean
  cost: number           # valor total
  savings: number        # economia vs tarifa cheia
  purpose: string        # ex: "reuniao com cliente", "treinamento"
```

## Despesas

```
expense:
  employee_id: string
  trip_id: string
  category: string       # "hospedagem" | "alimentacao" | "transporte" | "outros"
  amount: number
  date: date
  approved: boolean
  in_policy: boolean
  receipt: boolean
```

## Resumos Mensais (para Capsula)

```
monthly_summary:
  employee_id: string
  month: string
  trips_count: number
  total_spent: number
  savings: number
  compliance_rate: number
  top_destination: string
  avg_advance_days: number
```

## Regras de Consistencia

- Totais da visao consolidada (gestor) devem bater com a soma dos individuais
- Cada colaborador deve ter pelo menos 6 viagens no ano (para wrapped) e 1-3 no mes (para capsula)
- Pelo menos 1 colaborador deve ter compliance baixo (oportunidade de coaching)
- Pelo menos 1 colaborador deve ter compliance exemplar (oportunidade de reconhecimento)
- Destinos devem incluir mix de capitais brasileiras reais (SP, RJ, BH, BSB, CWB, POA)
