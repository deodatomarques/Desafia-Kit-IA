# ALTMET AI — Protocolo de Pesquisa Exploratória 0.1

**Versão:** 0.1  
**Escopo:** ações integrantes do IBOV e SMLL; candles de cinco minutos.  
**Natureza:** pesquisa exploratória, sem recomendação ou simulação operacional.

## 1. Pergunta inicial

Existem comportamentos intradiários recorrentes, identificáveis em candles de cinco minutos, nas ações integrantes do IBOV e do SMLL?

A pergunta é ampla e deve ser desdobrada em hipóteses específicas antes de qualquer teste confirmatório.

## 2. Objetivo desta etapa

Conhecer a estrutura dos dados, identificar padrões candidatos e formular hipóteses mensuráveis. A etapa não pretende demonstrar rentabilidade nem selecionar estratégias para execução.

## 3. Universo

- Ações integrantes do IBOV e do SMLL.
- Priorizar composição histórica dos índices por data.
- Registrar ticker, período de elegibilidade e eventuais mudanças de composição.
- Identificar sobreposição entre índices para evitar contar o mesmo ativo como observações independentes em análises agregadas.

A fonte oficial ou licenciada para a composição histórica ainda será definida.

## 4. Dados pretendidos

Campos mínimos por candle:

| Campo | Descrição |
|---|---|
| ativo | Código do ativo |
| timestamp | Data e hora de referência |
| open | Preço de abertura |
| high | Preço máximo |
| low | Preço mínimo |
| close | Preço de fechamento |
| volume | Volume negociado, com unidade documentada |

Metadados necessários: fonte, licença, fuso horário, calendário de negociação, ajustes corporativos, critérios de consolidação e período coberto.

A frequência pretendida é de cinco minutos. Deve-se esclarecer se timestamps representam início ou fim do intervalo.

## 5. Decisões pendentes antes da execução

1. Fonte de dados intradiários e condições de uso.
2. Período histórico disponível e suficiente.
3. Método de obtenção e armazenamento.
4. Tratamento de leilões, interrupções e alterações de horário.
5. Política de ajuste de eventos corporativos.
6. Definição formal do primeiro padrão a investigar.
7. Variável ou métrica primária.
8. Critérios de exclusão e tratamento de dados ausentes.

Não iniciar testes que dependam dessas decisões sem documentar as escolhas.

## 6. Etapas exploratórias

### Etapa A — Inventário e qualidade
Mapear cobertura por ativo e data; verificar integridade, lacunas, duplicidades, consistência OHLCV e eventos corporativos. Produzir relatório de qualidade antes de procurar padrões.

### Etapa B — Descrição
Descrever distribuição de retornos, amplitudes, volumes, frequência de observações e diferenças entre horários, ativos e períodos. Informar denominadores e limitações.

### Etapa C — Hipóteses candidatas
Registrar cada hipótese em ficha própria:
- ID e versão;
- motivação;
- definição operacional;
- hipótese nula e alternativa;
- variáveis e horizonte;
- população e período;
- filtros;
- métrica primária;
- método de análise;
- limitações e explicações alternativas.

### Etapa D — Exploração controlada
Explorar padrões e relações sem utilizar os resultados como confirmação. Registrar todas as famílias de testes realizadas e mudanças de parâmetros. Resultados descobertos nesta etapa são geradores de hipótese.

### Etapa E — Encaminhamento
Entregar dados, código ou procedimento reproduzível, ficha da hipótese e resultados completos ao Statistical Auditor.

## 7. Cuidados estatísticos

- Candles consecutivos podem apresentar dependência temporal.
- Ativos podem compartilhar fatores de mercado e não constituem observações independentes.
- Testes numerosos aumentam a probabilidade de falsos positivos.
- Resultados agregados podem esconder diferenças entre ativos e períodos.
- Eventos extremos podem dominar médias.
- A seleção atual de ativos pode introduzir viés de sobrevivência.

O método estatístico deve ser escolhido após a definição da hipótese e a inspeção das propriedades dos dados. Considerar correção de múltiplos testes e métodos de reamostragem compatíveis com dependência temporal.

## 8. Entregáveis

1. Inventário de dados e dicionário de campos.
2. Relatório de qualidade.
3. Fichas versionadas de hipóteses.
4. Relatório exploratório com resultados negativos e positivos.
5. Registro de parâmetros, filtros e decisões.
6. Pacote reproduzível para auditoria.

## 9. Critério de encerramento

A etapa exploratória termina quando houver dados caracterizados, hipóteses formalizadas e documentação suficiente para auditoria. Não termina com a identificação de um gráfico visualmente convincente.

## 10. Limite de interpretação

Nenhum achado exploratório deve ser comunicado como padrão comprovado, sinal de negociação ou vantagem econômica.
