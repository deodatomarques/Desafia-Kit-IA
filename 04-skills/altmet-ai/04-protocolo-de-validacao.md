# ALTMET AI — Protocolo de Validação 0.1

**Versão:** 0.1  
**Aplicação:** hipóteses originadas na pesquisa exploratória.  
**Status:** estrutura metodológica; parâmetros específicos serão definidos por hipótese.

## 1. Finalidade

Estabelecer condições para testar se um padrão candidato permanece observável em dados que não participaram de sua descoberta ou ajuste.

Validação estatística não equivale a rentabilidade, causalidade ou garantia de desempenho futuro.

## 2. Congelamento da hipótese

Antes da validação, registrar e congelar:

- ID e versão da hipótese;
- universo e período elegíveis;
- definição do padrão;
- variáveis e transformações;
- filtros e exclusões;
- métrica primária e métricas secundárias;
- método estatístico;
- critérios de avaliação;
- tratamento de dados ausentes;
- correção para múltiplas comparações, quando aplicável.

Mudanças posteriores devem gerar nova versão e não podem ser apresentadas como confirmação independente.

## 3. Separação temporal

Adotar separação cronológica, nunca aleatória por candle, para evitar vazamento temporal.

Estrutura conceitual:

1. **Exploração:** descoberta e formulação da hipótese.
2. **Desenvolvimento/ajuste:** estimativas e escolhas permitidas pelo protocolo.
3. **Validação:** avaliação em período posterior, reservado e não utilizado para ajustar a hipótese.
4. **Replicação:** teste em período adicional ou universo independente, quando viável.

As proporções e datas de cada janela permanecem pendentes até conhecermos a extensão, a qualidade e a cobertura do histórico. Não escolher divisões após observar qual delas produz o melhor resultado.

## 4. Integridade do conjunto reservado

- Manter o conjunto reservado inacessível durante a exploração.
- Não ajustar parâmetros com base nos resultados de validação.
- Registrar quem acessou os dados e quando.
- Se houver inspeção repetida ou ajuste motivado pelo conjunto reservado, reconhecer a contaminação e reservar novo período para confirmação.

## 5. Avaliação estatística

Conforme a hipótese, avaliar:

- tamanho do efeito e incerteza;
- intervalos de confiança;
- adequação e pressupostos dos testes;
- dependência temporal e entre ativos;
- múltiplas comparações;
- sensibilidade a períodos, ativos e parâmetros;
- estabilidade entre diferentes condições de mercado.

A métrica primária e o critério de avaliação devem ser definidos previamente. Resultados secundários e análises pós-hoc devem ser identificados como exploratórios.

## 6. Robustez e replicação

Verificar se o resultado:
- depende de um único ativo ou poucos eventos;
- permanece sob variações razoáveis previamente especificadas;
- é consistente em períodos distintos;
- é reproduzível a partir dos mesmos dados e procedimentos;
- desaparece quando se corrige um viés ou uma falha de dados.

Robustez não significa testar indefinidamente combinações até encontrar uma favorável. Cada família adicional de testes deve ser registrada.

## 7. Auditoria independente

O Statistical Auditor deve receber:
- protocolo congelado;
- identificação e proveniência dos dados;
- código ou procedimento reproduzível;
- resultados completos;
- registro de alterações;
- evidência de preservação do conjunto reservado.

O parecer deve indicar exatamente o que foi auditado e quais limitações permanecem.

## 8. Critérios de classificação

- **Não validado:** ainda não houve teste reservado adequado.
- **Inconclusivo:** evidência insuficiente ou imprecisa.
- **Não replicado:** resultado exploratório não se confirmou no teste.
- **Validado estatisticamente no escopo definido:** resultado consistente com o protocolo e aprovado em auditoria, limitado ao universo e período examinados.

Mesmo a última classificação não significa que exista vantagem operacional ou que o resultado continuará no futuro.

## 9. Etapa operacional futura — fora do escopo 0.1

Somente após evidência estatística suficiente poderá ser considerada uma etapa separada de avaliação operacional. Essa etapa exigirá regras de entrada e saída formalizadas, custos, emolumentos, spread, slippage, liquidez, capacidade, restrições de execução e testes adicionais. Nada disso será presumido nesta versão exploratória.

## 10. Princípio de validação

**A hipótese deve ser julgada por dados que não ajudaram a criá-la.**
