# ALTMET AI — Market Pattern Analyst

Pasta principal do projeto de agente de inteligência de mercado da ALTMET INVESTMENTS.

## Objetivo

Desenvolver, testar e evoluir um agente de IA para estudar padrões intradiários das ações negociadas na B3, produzindo análises fundamentadas em dados, evidências estatísticas e controles de risco.

## Princípios do projeto

- Preservação do capital em primeiro lugar.
- Liquidez e relação risco-retorno como critérios centrais.
- Análises baseadas em dados verificáveis; separar fatos, hipóteses e interpretações.
- Testes históricos e validação fora da amostra antes de considerar qualquer aplicação operacional.
- Nenhum envio automático de ordens: decisões e execução permanecem sob controle humano.
- Registrar versões, mudanças metodológicas, limitações e resultados.

## Escopo inicial

- Universo de estudo: ações integrantes do IBOV e do SMLL.
- Foco inicial: padrões intradiários.
- Dados e parâmetros experimentais serão documentados antes da implementação.
- A primeira etapa é experimental; resultados não constituem recomendação de investimento.

## Organização prevista

- `docs/` — visão do projeto, requisitos, arquitetura e decisões.
- `data/` — especificações, amostras permitidas e documentação das fontes; não armazenar credenciais ou dados licenciados sem autorização.
- `src/` — código do agente e módulos de análise.
- `tests/` — testes, validações e experimentos.
- `reports/` — relatórios e resultados de execução.

## Governança e segurança

- Nunca incluir senhas, tokens, chaves de API ou dados pessoais neste repositório.
- Verificar direitos de uso e limites das fontes de dados antes de coletar ou redistribuir informações.
- Não confundir correlação com causalidade nem desempenho histórico com garantia de resultado futuro.

## Histórico

Esta pasta passa a ser o espaço de trabalho dedicado ao Market Pattern Analyst. As versões do agente serão identificadas na documentação e no código, sem incorporar o número da versão ao nome da pasta.
