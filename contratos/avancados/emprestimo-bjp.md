# Contrato de Empréstimo com BJP

**Versão:** 1.0  
**Data:** [DATA_CONTRATO]  
**Protocolo:** PLS (PLIP-01)

## Partes

- **Credor:** [NOME_CREDOR], chave pública: [CHAVE_CREDOR]
- **Devedor:** [NOME_DEVEDOR], chave pública: [CHAVE_DEVEDOR]
- **Árbitro:** [NOME_ARBITRO], chave pública: [CHAVE_ARBITRO]

## Objetivo

Este contrato estabelece um empréstimo com colateral em Bitcoin através do [Bitcoin Justice Protocol (BJP)](https://github.com/PrivateLawSociety/pls-bjp), garantindo execução automática em caso de inadimplência.

## Termos do Empréstimo

### 1. Valores
- **Principal:** [VALOR_PRINCIPAL] BTC
- **Juros:** [TAXA_JUROS]% ao mês
- **Prazo:** [PRAZO_MESES] meses
- **Parcelas:** [NUMERO_PARCELAS] parcelas de [VALOR_PARCELA] BTC

### 2. Colateral BJP
- **Valor do Colateral:** [VALOR_COLATERAL] BTC
- **Multisig:** 2-de-3 (credor + devedor + árbitro)
- **Endereço:** [ENDERECO_MULTISIG]
- **Finalidade:** Garantia de pagamento

### 3. Cronograma
- **Data de Início:** [DATA_INICIO]
- **Data de Vencimento:** [DATA_VENCIMENTO]
- **Parcelas:** Mensais, vencimento no dia [DIA_VENCIMENTO]
- **Última Parcela:** [DATA_ULTIMA_PARCELA]

## Cláusulas Modulares

### Cláusula de Colateral
*[Incluir cláusula de colateral BJP - ver [clausulas/colateral.md](../../clausulas/colateral.md)]*

**Colateral:** [VALOR_COLATERAL] BTC em multisig 2-de-3

### Cláusula de Arbitragem
*[Incluir cláusula de arbitragem BJP - ver [clausulas/arbitragem.md](../../clausulas/arbitragem.md)]*

**Árbitro:** [NOME_ARBITRO] para disputas sobre pagamentos

### Cláusula de Comunicação
*[Incluir cláusula de comunicação BJP - ver [clausulas/comunicacao.md](../../clausulas/comunicacao.md)]*

**Plataforma:** [PLATAFORMA_COMUNICACAO] para notificações

## Fluxo de Execução BJP

### 1. Liberação Consensual
- **Ambas as Partes:** Credor e devedor podem liberar colateral
- **Pagamento Completo:** Colateral liberado após quitação
- **Renegociação:** Colateral liberado após acordo

### 2. Execução por Disputa
- **Inadimplência:** Devedor não paga no prazo
- **Notificação:** Credor notifica árbitro
- **Decisão:** Árbitro decide sobre execução
- **Execução:** Colateral executado conforme decisão

### 3. Execução Automática
- **Vencimento:** Parcela vencida há [DIAS_TOLERANCIA] dias
- **Notificação:** Sistema notifica automaticamente
- **Execução:** Colateral executado automaticamente
- **Distribuição:** Valores distribuídos conforme contrato

## Cálculos e Juros

### 1. Cálculo de Juros
- **Base:** Valor principal
- **Taxa:** [TAXA_JUROS]% ao mês
- **Capitalização:** Juros sobre juros
- **Fórmula:** P × (1 + i)^n

### 2. Tabela de Amortização
- **Parcela 1:** [VALOR_PARCELA_1] BTC (juros: [JUROS_1], principal: [PRINCIPAL_1])
- **Parcela 2:** [VALOR_PARCELA_2] BTC (juros: [JUROS_2], principal: [PRINCIPAL_2])
- **Parcela 3:** [VALOR_PARCELA_3] BTC (juros: [JUROS_3], principal: [PRINCIPAL_3])
- **Total:** [VALOR_TOTAL] BTC (juros: [TOTAL_JUROS], principal: [VALOR_PRINCIPAL])

### 3. Multa por Atraso
- **Taxa:** [TAXA_MULTA]% ao dia
- **Limite:** [LIMITE_MULTA]% do valor da parcela
- **Aplicação:** A partir do 1º dia de atraso

## Garantias e Segurança

### 1. Garantias do Devedor
- **Colateral Real:** Bitcoin depositado em multisig
- **Reputação:** Histórico de transações
- **Referências:** Avaliações de outros credores
- **Documentação:** Comprovantes de renda/patrimônio

### 2. Segurança do Credor
- **Colateral Bloqueado:** Colateral não pode ser movido sem consenso
- **Execução Garantida:** Colateral pode ser executado em caso de inadimplência
- **Árbitro Independente:** Árbitro escolhido por consenso
- **Transparência:** Todas as transações são públicas

### 3. Segurança do Sistema
- **Multisig:** Requer múltiplas assinaturas
- **Árbitro:** Terceiro independente
- **Auditoria:** Todas as transações são auditáveis
- **Backup:** Múltiplos backups das chaves

## Cenários de Execução

### 1. Pagamento Normal
- **Devedor paga:** Parcela paga no prazo
- **Colateral mantido:** Colateral permanece bloqueado
- **Reputação:** Reputação do devedor aumenta
- **Continuidade:** Contrato continua normalmente

### 2. Atraso no Pagamento
- **Tolerância:** [DIAS_TOLERANCIA] dias de tolerância
- **Multa:** Multa aplicada após tolerância
- **Notificação:** Credor notifica árbitro
- **Negociação:** Tentativa de renegociação

### 3. Inadimplência
- **Vencimento:** Parcela vencida há mais de [DIAS_TOLERANCIA] dias
- **Execução:** Colateral executado automaticamente
- **Distribuição:** Valores distribuídos conforme contrato
- **Reputação:** Reputação do devedor diminui

### 4. Quitação Antecipada
- **Desconto:** Desconto de [DESCONTO_ANTECIPADO]% nos juros
- **Liberação:** Colateral liberado imediatamente
- **Reputação:** Reputação do devedor aumenta
- **Contrato:** Contrato finalizado

## Alterações ao Contrato

### 1. Renegociação
- **Proposta:** Qualquer parte pode propor alterações
- **Consenso:** Requer consenso de todas as partes
- **Árbitro:** Árbitro pode mediar negociação
- **Documentação:** Alterações devem ser documentadas

### 2. Prorrogação
- **Prazo:** Prorrogação de até [PRAZO_PRORROGACAO] meses
- **Juros:** Juros podem ser ajustados
- **Colateral:** Colateral pode ser ajustado
- **Aprovação:** Requer aprovação do árbitro

### 3. Rescisão
- **Motivos:** Inadimplência, violação de termos, acordo mútuo
- **Processo:** Notificação + prazo para correção
- **Execução:** Colateral executado conforme contrato
- **Liquidação:** Valores liquidados conforme contrato

## Assinaturas Digitais

### Credor
- **Chave pública:** [CHAVE_CREDOR]
- **Assinatura:** [ASSINATURA_CREDOR]
- **Data:** [DATA_ASSINATURA_CREDOR]

### Devedor
- **Chave pública:** [CHAVE_DEVEDOR]
- **Assinatura:** [ASSINATURA_DEVEDOR]
- **Data:** [DATA_ASSINATURA_DEVEDOR]

### Árbitro
- **Chave pública:** [CHAVE_ARBITRO]
- **Assinatura:** [ASSINATURA_ARBITRO]
- **Data:** [DATA_ASSINATURA_ARBITRO]

## Metadados do Contrato

### Hash do Documento
- **SHA256:** [HASH_DOCUMENTO]

### Endereço Multisig
- **Bitcoin:** [ENDERECO_MULTISIG]
- **Quorum:** 2-de-3
- **Chaves:** [CHAVE_CREDOR], [CHAVE_DEVEDOR], [CHAVE_ARBITRO]

### Timestamps
- **Criado:** [TIMESTAMP_CRIACAO]
- **Assinado:** [TIMESTAMP_ASSINATURA]
- **Vigência:** [TIMESTAMP_VIGENCIA]

## Variáveis de Template

- `[DATA_CONTRATO]`: Data de criação do contrato
- `[NOME_CREDOR]`: Nome ou pseudônimo do credor
- `[NOME_DEVEDOR]`: Nome ou pseudônimo do devedor
- `[NOME_ARBITRO]`: Nome ou pseudônimo do árbitro
- `[CHAVE_CREDOR]`: Chave pública do credor
- `[CHAVE_DEVEDOR]`: Chave pública do devedor
- `[CHAVE_ARBITRO]`: Chave pública do árbitro
- `[VALOR_PRINCIPAL]`: Valor principal em BTC
- `[TAXA_JUROS]`: Taxa de juros ao mês em %
- `[PRAZO_MESES]`: Prazo em meses
- `[NUMERO_PARCELAS]`: Número de parcelas
- `[VALOR_PARCELA]`: Valor de cada parcela em BTC
- `[VALOR_COLATERAL]`: Valor do colateral em BTC
- `[ENDERECO_MULTISIG]`: Endereço da multisig
- `[DATA_INICIO]`: Data de início
- `[DATA_VENCIMENTO]`: Data de vencimento
- `[DIA_VENCIMENTO]`: Dia do vencimento
- `[DATA_ULTIMA_PARCELA]`: Data da última parcela
- `[PLATAFORMA_COMUNICACAO]`: Plataforma de comunicação
- `[DIAS_TOLERANCIA]`: Dias de tolerância
- `[TAXA_MULTA]`: Taxa de multa ao dia em %
- `[LIMITE_MULTA]`: Limite da multa em %
- `[DESCONTO_ANTECIPADO]`: Desconto por quitação antecipada em %
- `[PRAZO_PRORROGACAO]`: Prazo máximo de prorrogação em meses
- `[ASSINATURA_CREDOR]`: Assinatura digital do credor
- `[ASSINATURA_DEVEDOR]`: Assinatura digital do devedor
- `[ASSINATURA_ARBITRO]`: Assinatura digital do árbitro
- `[DATA_ASSINATURA_CREDOR]`: Data de assinatura do credor
- `[DATA_ASSINATURA_DEVEDOR]`: Data de assinatura do devedor
- `[DATA_ASSINATURA_ARBITRO]`: Data de assinatura do árbitro
- `[HASH_DOCUMENTO]`: Hash SHA256 do documento
- `[TIMESTAMP_CRIACAO]`: Timestamp de criação
- `[TIMESTAMP_ASSINATURA]`: Timestamp de assinatura
- `[TIMESTAMP_VIGENCIA]`: Timestamp de vigência
