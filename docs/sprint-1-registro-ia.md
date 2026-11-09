# Sprint 1 — Registro de uso de IA

## Auditoria - Decisões sobre propostas do agente

| # | Work item | Proposta do agente (resumo) | Decisão | Motivo |
|------|-----------|-----------------------------|---------|--------|
| D1 | AB#35 · [BE] US-03 | Objetivo, história, cenários, contrato e verificação | Aceita | Segue o molde e cita os cenários corretos |
| D2 | AB#35 · [BE] US-03 | Escopo em camadas (domínio, persistência, serviço e controller) | Modificada | A arquitetura é por fatia vertical |
| D3 | AB#35 · [BE] US-03 | Exceção "salvo se indispensáveis" em Fora de escopo | Modificada | Brecha que amplia o escopo |
| D4 | AB#35 · [BE] US-03 | Ambiguidades 1, 2, 3, 5 e 7 (cenários da história, "contabilizado na base", catálogo, criar ou substituir, consulta sem cadastro) | Aceita | Lacunas reais; viram decisões da equipe e ajustes na história |
| D5 | AB#35] · [BE] US-03 | Ambiguidade 4 (formato do Registro Acadêmico) | Modificada | Só dígitos, guardado como texto, zeros à esquerda preservados e sem decompor o código, para não amarrar o sistema a uma unidade de ensino |
| D6 | AB#35 · [BE] US-03 | Ambiguidade 6 (contrato da API) | Rejeitada | É função da [ESP] |
| D7 | AB#35 · [BE] US-03 | Ambiguidade 8 (nomes dos testes) | Modificada | Basta a regra de correspondência por nome entre cenário e teste |
| D8 | AB#36 · [FE] US-03 | Estrutura geral da descrição | Aceita | Segue o molde |
| D9 | AB#36 · [FE] US-03 | "Pronto quando" com um teste de componente por cenário | Modificada | O molde de [FE] pede cenários contra a API integrada, operação por teclado e estados de sucesso, erro e vazio |
| D10 | AB#36 · [FE] US-03 | Ambiguidades 4 a 9 (rota, catálogo, erros por campo, validação, edição do RA e estados da tela) | Aceita | Viram regras definidas pela equipe |
| D11 | AB#36 · [FE] US-03 | Ambiguidades 1 e 2 (descrição e contrato) | Rejeitada | Descrição e contrato são desta etapa e da [ESP] |
| D12 | AB#36 · [FE] US-03 | Ambiguidade 3 (perfil ainda não cadastrado) | Modificada | A tela mostra o formulário em branco; o sinal da API fica para a [ESP] |
| D13 | AB#40 · [BE] US-04 | Estrutura geral e cenários 1 e 2 (1ª rodada) | Aceita | Segue o molde, mas estava incompleta, por leitura de história desatualizada |
| D14 | AB#40 · [BE] US-04 | Escopo em camadas (1ª rodada) | Modificada | A arquitetura é por fatia vertical |
| D15 | AB#40 · [BE] US-04 | Ambiguidades 1 a 6 e 8 (1ª rodada) | Aceita | Viram regras definidas pela equipe |
| D16 | AB#40 · [BE] US-04 | Ambiguidade 7, cruzamento de grupos (1ª rodada) | Modificada | O cruzamento é da US-06, no módulo grupos |
| D17 | AB#40 · [BE] US-04 | Ambiguidade 9, contrato (1ª rodada) | Rejeitada | É função da [ESP] |
| D18 | AB#40 · [BE] US-04 | Cenários 1 a 5 e estrutura geral (2ª rodada) | Aceita | Cobre a história atualizada |
| D19 | AB#40 · [BE] US-04 | Escopo em camadas (2ª rodada) | Modificada | A arquitetura é por fatia vertical |
| D20 | AB#40 · [BE] US-04 | Ambiguidades 1, 3, 4, 5, 7 e 9 (2ª rodada) | Rejeitada | Já decididas pela equipe e agora escritas na Task |
| D21 | AB#40 · [BE] US-04 | Ambiguidades 2, 6 e 10 (2ª rodada) | Aceita | Viram regras e escopo da Task |
| D22 | AB#40 · [BE] US-04 | Ambiguidade 8, representação do estado vazio (2ª rodada) | Modificada | Decisão da [ESP] |
| D23 | AB#41 · [FE] US-04 | Estrutura geral e cenários 1 a 5 | Aceita | Segue o molde |
| D24 | AB#41 · [FE] US-04 | Pasta `features/disponibilidade/` | Modificada | O front-end espelha os módulos: `features/perfil/disponibilidade/` |
| D25 | AB#41 · [FE] US-04 | "Pronto quando" com um teste de componente por cenário | Modificada | O molde de [FE] pede cenários contra a API integrada, operação por teclado e estados |
| D26 | AB#41 · [FE] US-04 | Ambiguidades 2, 5, 6, 7 e 8 (rota, substituição da grade, validação, estados e erros) | Aceita | Viram regras definidas pela equipe |
| D27 | AB#41 · [FE] US-04 | Ambiguidades 1, 3, 9, 10 e 11 | Rejeitada | Descrição e contrato são desta etapa e da [ESP], ou já foram decididas |
| D28 | AB#41 · [FE] US-04 | Ambiguidade 4 (estado vazio na API) | Modificada | O sinal da API é da [ESP] |
| D29 | AB#46 · [BE] US-06 (cenários 4 e 5) | Estrutura geral, cenários 4 e 5, dependência da AB#45 e proibição de `perfil.internal` | Aceita | Segue o molde e delimita bem o escopo e as fronteiras |
| D30 | AB#46 · [BE] US-06 (cenários 4 e 5) | Título alterado para "Filtrar grupos por modalidade e informar ausência de compatibilidade" | Modificada | Manter o título original da Task |
| D31 | AB#46 · [BE] US-06 (cenários 4 e 5) | Objetivo de "informar" a ausência de compatibilidade | Modificada | O back-end responde com lista vazia e sucesso; a mensagem é apresentada pela tela |
| D32 | AB#46 · [BE] US-06 (cenários 4 e 5) | Ambiguidade 1 (alterar a consulta da AB#45 ou criar nova operação) | Aceita | Estende a mesma consulta, depois da AB#45 integrada |
| D33 | AB#46 · [BE] US-06 (cenários 4 e 5) | Ambiguidades 2, 3 e 4 (regra de modalidade) | Aceita | "Ambos" casa com qualquer modalidade, as demais precisam ser iguais, e a comparação usa a faixa que contém o horário do grupo; o cenário 4 vira Esquema do Cenário com todas as combinações |
| D34 | AB#46 · [BE] US-06 (cenários 4 e 5) | Ambiguidades 5 e 6 (forma da resposta e dono da mensagem) | Aceita | Lista vazia com sucesso, sem erro de negócio; a mensagem fica no front-end |
| D35 | AB#46 · [BE] US-06 (cenários 4 e 5) | Ambiguidade 7 (cenário 5 com todos os filtros juntos) | Aceita | O teste usa grupos que falham, cada um, em um critério, sem nenhum que passe |
| D36 | AB#46 · [BE] US-06 (cenários 4 e 5) | Ambiguidade 8 (modalidade na resposta vazia) | Rejeitada | Lista vazia não tem itens; a modalidade já consta em cada grupo retornado, exigência da AB#45 |
| D37 | AB#46 · [BE] US-06 (cenários 4 e 5) | Ambiguidade 9 (grupo "aberto") | Aceita | Aberto significa com vaga; não há estado de encerramento nesta sprint, e o filtro é da AB#45 |
| D38 | AB#46 · [BE] US-06 (cenários 4 e 5) | Ambiguidade 10 (dados de exemplo) | Aceita | Os testes montam dados fictícios determinísticos; a migração só inclui grupos de cada modalidade, se preciso |

## Crítica do Plano Completo
| 08/11/2026 | Plano completo (P2) | Organização geral por história: [ESP], [BE], [FE], [VER] e [REV] | Aceita | O padrão se repete e segue o molde |
| 08/11/2026 | Plano completo (P2) | Falta de dependências formais entre as Tasks | Modificada | Vínculos Predecessor só onde há dependência real ([ESP] antes de [BE] e [FE]; [BE] das US-03 e US-04 antes do [BE] da US-06); a ordem de execução fica escrita no planejamento |
| 08/11/2026 | Plano completo (P2) | AB#50 não pertence a uma história | Rejeitada | É a Task de documentação do planejamento, criada fora da Sprint 1 por desenho do roteiro |
| 08/11/2026 | Plano completo (P2) | AB#50 sem seção Verificação | Modificada | Acrescentar apenas "Pronto quando": pull request com os arquivos de docs/ integrado no main, com CI verde |
| 08/11/2026 | Plano completo (P2) | [VER] e [REV] dependem de artefatos externos sem formato mínimo | Modificada | O formato já existe no roteiro (13.5); será copiado para a descrição das Tasks |
| 08/11/2026 | Plano completo (P2) | AB#34, AB#39 e AB#44: verificação por "ausência de dúvidas" | Aceita | A [ESP] precisa de lista objetiva: operação, entrada, saída e erro para cada cenário |
| 08/11/2026 | Plano completo (P2) | AB#47: verificação subjetiva e sem estados de erro e vazio | Aceita | Usar a verificação do molde de [FE] |
| 08/11/2026 | Plano completo (P2) | [VER] e [REV] fora da estrutura Comando e Pronto quando | Modificada | Mantêm a natureza própria, com "Pronto quando" explícito e sem comando |
| 08/11/2026 | Plano completo (P2) | Dividir a AB#45 em três Tasks (consulta, integração com perfil, dados fictícios) | Rejeitada | A divisão proposta é por camada, contra a regra de tarefas verticais; a Task tem 5h, abaixo do limite de 8h, e a US-06 já tem dois [BE] |
| 08/11/2026 | Plano completo (P2) | AB#47, AB#40 e AB#41 grandes demais | Rejeitada | Todas estão abaixo de 8h, e as regras de cada uma estão cobertas por cenários |
| 08/11/2026 | Plano completo (P2) | Separar o catálogo de cursos e disciplinas da AB#35 | Rejeitada | Seria uma Task horizontal, sem cenário próprio; os cenários da US-03 dependem do catálogo |
| 08/11/2026 | Plano completo (P2) | Risco de fronteira na AB#45 (uso de perfil.internal) | Aceita | O escopo passa a permitir só a API pública do módulo perfil, por chamada síncrona, sem dependência inversa |
| 08/11/2026 | Plano completo (P2) | AB#35 e AB#40 expondo APIs públicas | Aceita | Expor o mínimo: interfaces e records públicos, sem entidades JPA, repositórios ou DTOs internos |
| 08/11/2026 | Plano completo (P2) | Contrato sem distinguir API HTTP e API pública entre módulos | Aceita | A [ESP] registra os dois em seções separadas |
| 08/11/2026 | Plano completo (P2) | Fronteira no front-end: acesso só pela porta index.ts | Aceita | Regra acrescentada às Tasks [FE] AB#36, AB#41 e AB#47 |
| 08/11/2026 | Plano completo (P2) | Cenários 4 e 5 da US-06 sem Task | Modificada | Conferir a AB#46, que não apareceu na análise; completar AB#44, AB#47, AB#48 e AB#49 com os cenários 4 e 5; os cenários não são removidos |
| 08/11/2026 | Plano completo (P2) | Testes de componente por cenário nas Tasks [FE] | Rejeitada | O roteiro os considera bem-vindos, mas não obrigatórios |
| 08/11/2026 | Plano completo (P2) | `.\verificar.ps1 frontend` não substitui a verificação completa | Modificada | O parcial serve à iteração; o "Pronto quando" exige o `.\verificar.ps1` completo antes do pull request |
