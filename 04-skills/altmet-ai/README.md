# ALTMET AI — Pesquisa de Padrões de Mercado

**Pacote documental:** versão 0.1  
**Universo inicial:** ações do IBOV e SMLL  
**Periodicidade pretendida:** candles de cinco minutos  
**Status:** especificação documental concluída; implementação e experimento dependem de decisões e dados.

## Componentes

| Arquivo | Função |
|---|---|
| [01 — Market Pattern Researcher](01-market-pattern-researcher.md) | Pesquisa exploratória, formula hipóteses e documenta resultados. |
| [02 — Statistical Auditor](02-statistical-auditor.md) | Audita independentemente dados, métodos e conclusões. |
| [03 — Protocolo de Pesquisa Exploratória](03-protocolo-de-pesquisa-exploratoria.md) | Define o processo de descoberta e documentação. |
| [04 — Protocolo de Validação](04-protocolo-de-validacao.md) | Define a separação temporal e os critérios de validação. |

## Fluxo

1. Definir a pergunta de pesquisa.
2. Obter e validar os dados.
3. Formalizar hipótese e critérios.
4. Realizar análise exploratória.
5. Encaminhar materiais ao auditor.
6. Corrigir fragilidades e congelar a hipótese.
7. Executar validação temporal reservada.
8. Registrar parecer e limitações.

## Decisões ainda pendentes

- fornecedor/fonte dos dados intradiários e licença de uso;
- período histórico e cobertura;
- método de armazenamento e atualização;
- política de eventos corporativos e leilões;
- primeira hipótese específica;
- métricas e testes adequados a essa hipótese;
- datas ou proporções das janelas temporais.

Essas decisões não foram preenchidas por suposição. Devem ser tomadas antes da execução do experimento.

## Limites da versão 0.1

Esta versão não fornece sinais de compra ou venda, não recomenda ativos e não afirma rentabilidade. O objetivo é investigar padrões com rastreabilidade e rigor metodológico.

**Princípio:** descoberta não é validação; validação estatística não é garantia de vantagem operacional.
