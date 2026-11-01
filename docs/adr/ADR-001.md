# ADR-001 — Estilo Arquitetural

- **Situação:** Aceita 
- **Data:** 27/10/2026
- **Participantes:** Enrico Reis, Leandro Torres, Marcio Camargos, Richard Ribeiro e Suzane Andrade

## Contexto

O Connexa é uma plataforma que forma grupos de estudo entre estudantes compatíveis e mostra à coordenação e à monitoria quais grupos existem e estão ativos, substituindo planilhas e o cruzamento manual de horários.
- Identidade e LGPD: e-mail institucional comprovado, senha sob guarda do Connexa e dados pessoais com dono e finalidade claros.
- Acessibilidade e celular: uso por teclado e leitor de tela (WCAG), com a maior parte do acesso pelo celular.
- Prazo, equipe e carga: 1 semestre, 5 integrantes.
- Agente de IA: o código é escrito em tarefas verticais, exigindo fronteiras explícitas e verificáveis.

## Decisão

- Estilo: monolito modular com fatias verticais, com um módulo por território do escopo mais o módulo comum.
- Back-end: Java 21 com Spring Boot e Spring Modulith, que verifica as fronteiras no build.
- Dados: PostgreSQL com um schema por módulo e migrações versionadas com Flyway.
- Front-end: SPA em React + TypeScript, organizada por funcionalidade, responsiva e acessível.
- Regra geral: toda regra de negócio e de segurança fica no back-end, e o código fica em um único repositório.

## Alternativas consideradas

| Alternativa | Por que não foi escolhida |
|---|---|
| Camadas puras (MVC) | Mudanças atravessam todas as camadas e as fronteiras de negócio não aparecem na estrutura |
| Microsserviços | Equipe pequena, um semestre para execução |
| C# / .NET | Menor familiaridade com C# e .NET |
| TypeScript / NestJS | Menor prática com NestJS no back-end |

## Consequências

- **Positivas:** um deploy por camada, transações simples, mudanças localizadas por funcionalidade e escopo claro para o agente.
- **Negativas:** escala como bloco único e exige disciplina contra duplicação entre fatias.
- **Como verificar:** o teste do Spring Modulith e o CI rodam em todo pull request, e o main bloqueia integração com CI vermelho; reavaliar com novo ADR se um módulo exigir escala.
