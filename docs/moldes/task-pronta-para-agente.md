Título: [BE] <verbo> <resultado observável> — <história, em poucas palavras>

## Objetivo
<Uma frase: o que passa a funcionar quando esta Task terminar.>

## História e cenários
História: AB#<id da história>
Cenários cobertos por esta Task: <nomes exatos dos cenários Gherkin>
Cenários fora desta Task: <quais e por quê>

## Contrato  (preenchido pela Task [ESP])
Operação: <verbo HTTP> <rota>
Entrada: <campos, tipos e obrigatoriedade>
Saída: <campos>
Erros: <código de resposta> quando <situação> → cenário "<nome>"

## Escopo
Pode alterar: <módulo e pastas>
Pode usar sem alterar: <API pública de outro módulo, se necessária>
Não pode alterar: testes existentes, CI, configuração de fronteiras,
                  dependências do projeto, outros módulos

## Verificação
Comando: <comando-de-verificacao>
Pronto quando: os testes de aceitação dos cenários acima passam
e nenhuma verificação existente falha.

## Fora de escopo
<O que o agente não deve fazer, mesmo que pareça útil.>
