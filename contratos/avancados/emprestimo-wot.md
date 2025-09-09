# Contrato de Empréstimo com Web of Trust (WoT)

**Versão:** 1.0  
**Data:** [DATA_CONTRATO]  
**Protocolo:** PLS (PLIP-01) + WoT

## Partes

- **Credor:** [NOME_CREDOR], chave pública: [CHAVE_CREDOR], reputação: [REPUTACAO_CREDOR] pontos
- **Devedor:** [NOME_DEVEDOR], chave pública: [CHAVE_DEVEDOR], reputação: [REPUTACAO_DEVEDOR] pontos
- **Árbitro:** [NOME_ARBITRO], chave pública: [CHAVE_ARBITRO], reputação: [REPUTACAO_ARBITRO] pontos

## Termos do Empréstimo

### 1. Valor e Condições
- **Valor emprestado:** [VALOR_EMPRESTIMO] [MOEDA_EMPRESTIMO]
- **Colateral base:** [COLATERAL_BASE_BTC] BTC
- **Colateral ajustado:** [COLATERAL_AJUSTADO_BTC] BTC (após redução por reputação)
- **Taxa de juros:** [TAXA_JUROS]% ao mês
- **Prazo:** [PRAZO_DIAS] dias
- **Data de vencimento:** [DATA_VENCIMENTO]

### 2. Benefícios por Reputação
- **Redução de colateral:** [PERCENTUAL_REDUCAO]% (devido à alta reputação)
- **Taxa de juros reduzida:** [TAXA_JUROS_REDUZIDA]% (benefício premium)
- **Prioridade na arbitragem:** Sim (reputação > 75 pontos)

## Cláusulas Modulares

### Cláusula de Colateral com WoT
*[Incluir cláusula de colateral ajustado por reputação - ver [clausulas/colateral.md](../../clausulas/colateral.md)]*

**Cálculo do colateral:**
```
Colateral Final = [COLATERAL_BASE_BTC] BTC × (1 - [PERCENTUAL_REDUCAO]%)
Colateral Final = [COLATERAL_AJUSTADO_BTC] BTC
```

### Cláusula de Reputação
*[Incluir cláusula de reputação completa - ver [clausulas/reputacao.md](../../clausulas/reputacao.md)]*

**Verificação de reputação:**
- Plataforma: [PLATAFORMA_WOT]
- Reputação mínima: [REPUTACAO_MINIMA] pontos
- Benefícios aplicados: Redução de colateral e taxa de juros

### Cláusula de Arbitragem
*[Incluir cláusula de arbitragem básica - ver [clausulas/arbitragem.md](../../clausulas/arbitragem.md)]*

**Árbitro premium:** [NOME_ARBITRO] com reputação de [REPUTACAO_ARBITRO] pontos

### Cláusula de Comunicação
*[Incluir cláusula de comunicação básica - ver [clausulas/comunicacao.md](../../clausulas/comunicacao.md)]*

**Plataforma:** [PLATAFORMA_COMUNICACAO] com integração WoT

## Mecânica de Execução

### 1. Verificação de Reputação
1. Reputação verificada em [PLATAFORMA_WOT]
2. Benefícios calculados automaticamente
3. Colateral ajustado conforme reputação

### 2. Assinatura e Depósito
1. Contrato assinado via [PLATAFORMA_ASSINATURA]
2. Colateral ajustado ([COLATERAL_AJUSTADO_BTC] BTC) depositado em [ENDERECO_MULTISIG]
3. Empréstimo liberado pelo credor

### 3. Pagamento e Liberação
1. Pagamento devido em [DATA_VENCIMENTO]
2. Colateral devolvido após quitação
3. Reputação atualizada positivamente

### 4. Disputas
1. Disputas resolvidas por [NOME_ARBITRO] (prioridade por reputação)
2. Evidências via [PLATAFORMA_COMUNICACAO]
3. Decisão em até 14 dias

## Atualização de Reputação

### Sucesso do Contrato
- **Credor:** +[PONTO_SUCESSO_CREDOR] pontos
- **Devedor:** +[PONTO_SUCESSO_DEVEDOR] pontos
- **Árbitro:** +[PONTO_SUCESSO_ARBITRO] pontos (se envolvido)

### Falha do Contrato
- **Parte em falta:** -[PONTO_FALHA] pontos
- **Parte prejudicada:** +[PONTO_COMPENSACAO] pontos
- **Árbitro:** +[PONTO_DECISAO_JUSTA] pontos

## Benefícios Especiais

### Para Credores com Alta Reputação
- Taxa de juros reduzida
- Prioridade na escolha de devedores
- Acesso a contratos de maior valor

### Para Devedores com Alta Reputação
- Colateral reduzido
- Taxa de juros preferencial
- Processo de aprovação acelerado

### Para Árbitros com Alta Reputação
- Prioridade na escolha
- Taxas de arbitragem premium
- Acesso a disputas de alto valor

## Riscos e Limitações

### Risco de Flutuação
- Flutuação de preço é risco mútuo
- Não sujeito a arbitragem
- Aceito por ambas as partes

### Limitações do WoT
- Reputação pode mudar durante o contrato
- Benefícios baseados na reputação no momento da assinatura
- Atualizações de reputação não afetam contratos em vigor

## Assinaturas Digitais

### Credor
- **Chave pública:** [CHAVE_CREDOR]
- **Reputação:** [REPUTACAO_CREDOR] pontos
- **Assinatura:** [ASSINATURA_CREDOR]
- **Data:** [DATA_ASSINATURA_CREDOR]

### Devedor
- **Chave pública:** [CHAVE_DEVEDOR]
- **Reputação:** [REPUTACAO_DEVEDOR] pontos
- **Assinatura:** [ASSINATURA_DEVEDOR]
- **Data:** [DATA_ASSINATURA_DEVEDOR]

### Árbitro
- **Chave pública:** [CHAVE_ARBITRO]
- **Reputação:** [REPUTACAO_ARBITRO] pontos
- **Assinatura:** [ASSINATURA_ARBITRO]
- **Data:** [DATA_ASSINATURA_ARBITRO]

## Metadados do Contrato

### Hash do Documento
- **SHA256:** [HASH_DOCUMENTO]

### Endereço Multisig
- **Bitcoin:** [ENDERECO_MULTISIG]
- **Quorum:** 2-de-3
- **Chaves:** [CHAVE_DEVEDOR], [CHAVE_CREDOR], [CHAVE_ARBITRO]

### Reputação no Momento da Assinatura
- **Credor:** [REPUTACAO_CREDOR] pontos
- **Devedor:** [REPUTACAO_DEVEDOR] pontos
- **Árbitro:** [REPUTACAO_ARBITRO] pontos

### Timestamps
- **Criado:** [TIMESTAMP_CRIACAO]
- **Assinado:** [TIMESTAMP_ASSINATURA]
- **Vencimento:** [TIMESTAMP_VENCIMENTO]

## Variáveis de Template

- `[DATA_CONTRATO]`: Data de criação do contrato
- `[NOME_CREDOR]`: Nome ou pseudônimo do credor
- `[NOME_DEVEDOR]`: Nome ou pseudônimo do devedor
- `[NOME_ARBITRO]`: Nome ou pseudônimo do árbitro
- `[CHAVE_CREDOR]`: Chave pública do credor
- `[CHAVE_DEVEDOR]`: Chave pública do devedor
- `[CHAVE_ARBITRO]`: Chave pública do árbitro
- `[REPUTACAO_CREDOR]`: Reputação do credor em pontos
- `[REPUTACAO_DEVEDOR]`: Reputação do devedor em pontos
- `[REPUTACAO_ARBITRO]`: Reputação do árbitro em pontos
- `[VALOR_EMPRESTIMO]`: Valor do empréstimo
- `[MOEDA_EMPRESTIMO]`: Moeda do empréstimo
- `[COLATERAL_BASE_BTC]`: Colateral base em Bitcoin
- `[COLATERAL_AJUSTADO_BTC]`: Colateral ajustado em Bitcoin
- `[TAXA_JUROS]`: Taxa de juros mensal
- `[TAXA_JUROS_REDUZIDA]`: Taxa de juros reduzida
- `[PRAZO_DIAS]`: Prazo em dias
- `[DATA_VENCIMENTO]`: Data de vencimento
- `[PERCENTUAL_REDUCAO]`: Percentual de redução de colateral
- `[PLATAFORMA_WOT]`: Plataforma Web of Trust
- `[REPUTACAO_MINIMA]`: Reputação mínima necessária
- `[PLATAFORMA_COMUNICACAO]`: Plataforma de comunicação
- `[PLATAFORMA_ASSINATURA]`: Plataforma de assinatura
- `[PONTO_SUCESSO_CREDOR]`: Pontos por sucesso (credor)
- `[PONTO_SUCESSO_DEVEDOR]`: Pontos por sucesso (devedor)
- `[PONTO_SUCESSO_ARBITRO]`: Pontos por sucesso (árbitro)
- `[PONTO_FALHA]`: Pontos perdidos por falha
- `[PONTO_COMPENSACAO]`: Pontos por compensação
- `[PONTO_DECISAO_JUSTA]`: Pontos por decisão justa
- `[ASSINATURA_CREDOR]`: Assinatura digital do credor
- `[ASSINATURA_DEVEDOR]`: Assinatura digital do devedor
- `[ASSINATURA_ARBITRO]`: Assinatura digital do árbitro
- `[DATA_ASSINATURA_CREDOR]`: Data de assinatura do credor
- `[DATA_ASSINATURA_DEVEDOR]`: Data de assinatura do devedor
- `[DATA_ASSINATURA_ARBITRO]`: Data de assinatura do árbitro
- `[HASH_DOCUMENTO]`: Hash SHA256 do documento
- `[ENDERECO_MULTISIG]`: Endereço da multisig
- `[TIMESTAMP_CRIACAO]`: Timestamp de criação
- `[TIMESTAMP_ASSINATURA]`: Timestamp de assinatura
- `[TIMESTAMP_VENCIMENTO]`: Timestamp de vencimento
