# Sprint 1 — Planejamento

## 1. Meta da sprint
Ao final desta sprint, um estudante consegue informar suas disciplinas e horários livres e ver os grupos de estudo compatíveis.

## 2. Conta da capacidade
5 integrantes, 3 semanas
Horas por integrante, por semana ...  8h
Integrantes ........................   5
Semanas ............................   3
Capacidade bruta ...................  120h
( - ) reserva de 20% ...............  24h
( - ) reuniões da equipe ...........   4h
Capacidade de planejamento .........  92h
Alvo da primeira sprint (75%) ......  69h

## 3. Justificativa da seleção

**Histórias selecionadas**

| História | Pontos | Como sustenta a meta |
|----------|--------|----------------------|
| US-03 Cadastrar as disciplinas cursadas no semestre | 2 | O estudante informa suas disciplinas |
| US-04 Declarar horários de disponibilidade semanal | 3 | O estudante informa seus horários livres |
| US-06 Ver grupos sugeridos por disciplina e horário compatível | 8 | O estudante vê os grupos de estudo compatíveis |

As três formam uma fatia vertical completa (tela, API e banco) e dependem umas das outras: a US-06 cruza as disciplinas da US-03 com os horários da US-04.

**Histórias puladas e motivo**

| História | Motivo |
|----------|--------|
| US-01, US-18 e US-02 | Histórias do território de identidade ficam fora da Sprint 1 |
| US-09 Criar um novo grupo de estudo | A meta não inclui criar grupos. Para a demonstração, a US-06 inicia com gurpos já existentes |
| US-08 Entrar em um grupo sugerido | A meta termina em ver os grupos compatíveis; entrar fica para a próxima sprint |
| US-05 e US-07 | Complementares: não são necessárias para a meta |
| Demais histórias (encontros, acompanhamento e painel) | Não sustentam a meta desta sprint |

## 4. Esqueleto de tarefas
Esforço humano estimado em horas, no campo `Remaining Work`. Nenhuma Task passa de 8h.

### US-03 — Cadastrar as disciplinas cursadas no semestre

| Prefixo | Título da Task | Horas |
|---------|----------------|-------|
| [ESP] | Especificar o contrato do cadastro de perfil acadêmico — US-03 | 1 |
| [BE] | Salvar e consultar perfil acadêmico com disciplinas do semestre — US-03 | 3 |
| [FE] | Tela de cadastro de perfil acadêmico — US-03 | 3 |
| [VER] | Executar manualmente os cenários da US-03 | 1 |
| [REV] | Revisar os pull requests da US-03 por evidências | 1 |

### US-04 — Declarar horários de disponibilidade semanal

| Prefixo | Título da Task | Horas |
|---------|----------------|-------|
| [ESP] | Especificar o contrato da disponibilidade semanal — US-04 | 1 |
| [BE] | Salvar e consultar a grade de disponibilidade semanal — US-04 | 4 |
| [FE] | Tela de disponibilidade semanal — US-04 | 4 |
| [VER] | Executar manualmente os cenários da US-04 | 2 |
| [REV] | Revisar os pull requests da US-04 por evidências | 1 |

### US-06 — Ver grupos sugeridos por disciplina e horário compatível

| Prefixo | Título da Task | Horas |
|---------|----------------|-------|
| [ESP] | Especificar o contrato da listagem de grupos compatíveis — US-06 | 2 |
| [BE] | Listar grupos compatíveis por disciplina, horário e vagas, com grupos de exemplo — US-06 (cenários 1, 2 e 3) | 5 |
| [BE] | Filtrar por modalidade e informar ausência de grupos compatíveis — US-06 (cenários 4 e 5) | 3 |
| [FE] | Tela de sugestões de grupos — US-06 | 5 |
| [VER] | Executar manualmente os cenários da US-06 | 2 |
| [REV] | Revisar os pull requests da US-06 por evidências | 2 |

**Total estimado:** 40h em 16 Tasks.


## 5. Riscos e resposta prevista

## 12.2 Mapeamento de Riscos e Mitigações

| ID | Risco | Impacto | Probabilidade | Plano de Mitigação |
|---|---|---|---|---|
| R01 | **Atuação do Agente de IA:** O agente gerar código incompatível com a arquitetura do projeto ou contratos incorretos. | Alto | Média | Auditar previamente a especificação do contrato (`[ESP]`) via MCP antes das implementações de Back-end e Front-end. |
| R02 | **Sobrecarga de Tarefas:** Concentração de estimativas de desenvolvimento em poucos integrantes. | Médio | Alta | Balancear contínua e claramente as atribuições na aba *Capacity* do Azure Boards. |
| R03 | **Conflitos de Merge:** Dessincronização entre as branches locais e a branch `main`. | Médio | Média | Executar `git fetch` frequentemente e manter Pull Requests pequenos e focados. |

## 6. Definition of Done

[PREENCHER na Etapa 12: ponto de partida do roteiro (12.3), com os itens que a equipe acrescentar.]

## 7. Registro da reunião de planejamento

- **Data:** 07/11/2026
- **Duração:** 4h
- **Participantes:** Todos os integrantes
