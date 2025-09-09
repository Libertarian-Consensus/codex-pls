# Contrato de Empréstimo Híbrido (WoT + BJP + Seguro)

**Versão:** 1.0  
**Data:** [DATA_CONTRATO]  
**Protocolo:** PLS (PLIP-01) + WoT + BJP + Seguro

## Partes

- **Credor:** [NOME_CREDOR], chave pública: [CHAVE_CREDOR], reputação: [REPUTACAO_CREDOR] pontos
- **Devedor:** [NOME_DEVEDOR], chave pública: [CHAVE_DEVEDOR], reputação: [REPUTACAO_DEVEDOR] pontos
- **Árbitro:** [NOME_ARBITRO], chave pública: [CHAVE_ARBITRO], reputação: [REPUTACAO_ARBITRO] pontos

## Termos do Empréstimo

### 1. Valor e Condições
- **Valor emprestado:** [VALOR_EMPRESTIMO] [MOEDA_EMPRESTIMO]
- **Colateral base:** [COLATERAL_BASE_BTC] BTC
- **Colateral final:** [COLATERAL_FINAL_BTC] BTC (após todas as reduções)
- **Taxa de juros:** [TAXA_JUROS]% ao mês
- **Prazo:** [PRAZO_DIAS] dias
- **Data de vencimento:** [DATA_VENCIMENTO]

### 2. Redutores de Risco Aplicados
- **Redução por reputação:** [PERCENTUAL_REDUCAO_REPUTACAO]%
- **Redução por seguro:** [PERCENTUAL_REDUCAO_SEGURO]%
- **Redução por associação:** [PERCENTUAL_REDUCAO_ASSOCIACAO]%
- **Redução total:** [PERCENTUAL_REDUCAO_TOTAL]%

### 3. Cálculo do Colateral
```
Colateral Final = [COLATERAL_BASE_BTC] BTC × (1 - [PERCENTUAL_REDUCAO_TOTAL]%)
Colateral Final = [COLATERAL_FINAL_BTC] BTC
```

## Cláusulas Modulares

### Cláusula de Colateral Híbrido
*[Incluir cláusula de colateral híbrido - ver [clausulas/colateral.md](../../clausulas/colateral.md)]*

**Múltiplas reduções aplicadas:**
- Reputação: [PERCENTUAL_REDUCAO_REPUTACAO]%
- Seguro: [PERCENTUAL_REDUCAO_SEGURO]%
- Associação: [PERCENTUAL_REDUCAO_ASSOCIACAO]%
- Total: [PERCENTUAL_REDUCAO_TOTAL]%

### Cláusula de Reputação
*[Incluir cláusula de reputação completa - ver [clausulas/reputacao.md](../../clausulas/reputacao.md)]*

**Verificação de reputação:**
- Plataforma: [PLATAFORMA_WOT]
- Reputação mínima: [REPUTACAO_MINIMA] pontos
- Benefícios aplicados: Redução de colateral

### Cláusula de Seguro
*[Incluir cláusula de seguro completa - ver [clausulas/seguro.md](../../clausulas/seguro.md)]*

**Cobertura do fundo de seguro:**
- Taxa paga: [TAXA_SEGURO]% sobre [VALOR_EMPRESTIMO]
- Redução de colateral: [PERCENTUAL_REDUCAO_SEGURO]%
- Cobertura máxima: [LIMITE_COBERTURA] BTC

### Cláusula de Arbitragem
*[Incluir cláusula de arbitragem básica - ver [clausulas/arbitragem.md](../../clausulas/arbitragem.md)]*

**Árbitro premium:** [NOME_ARBITRO] com reputação de [REPUTACAO_ARBITRO] pontos

### Cláusula de Comunicação
*[Incluir cláusula de comunicação básica - ver [clausulas/comunicacao.md](../../clausulas/comunicacao.md)]*

**Plataforma:** [PLATAFORMA_COMUNICACAO] com integração WoT e BJP

## Mecânica de Execução

### 1. Verificação de Elegibilidade
1. Reputação verificada em [PLATAFORMA_WOT]
2. Participação no fundo de seguro confirmada
3. Associação à [NOME_ASSOCIACAO] verificada
4. Benefícios calculados automaticamente

### 2. Assinatura e Depósito
1. Contrato assinado via [PLATAFORMA_ASSINATURA]
2. Taxa de seguro ([TAXA_SEGURO]%) depositada em [ENDERECO_FUNDO]
3. Colateral final ([COLATERAL_FINAL_BTC] BTC) depositado em [ENDERECO_MULTISIG]
4. Empréstimo liberado pelo credor

### 3. Pagamento e Liberação
1. Pagamento devido em [DATA_VENCIMENTO]
2. Colateral devolvido após quitação
3. Reputação atualizada positivamente
4. Seguro mantido para futuros contratos

### 4. Disputas
1. Disputas resolvidas por [NOME_ARBITRO] (prioridade por reputação)
2. Evidências via [PLATAFORMA_COMUNICACAO]
3. Decisão em até 14 dias
4. Cobertura de seguro aplicável se necessário

## Benefícios Combinados

### Para Partes com Alta Reputação
- Colateral reduzido por reputação
- Taxa de juros preferencial
- Prioridade na arbitragem
- Acesso a contratos de maior valor

### Para Participantes do Seguro
- Colateral reduzido por seguro
- Cobertura de perdas
- Custos de arbitragem cobertos
- Proteção contra inadimplência

### Para Membros da Associação
- Colateral reduzido por associação
- Acesso a rede de confiança
- Suporte da comunidade
- Benefícios exclusivos

## Atualização de Reputação

### Sucesso do Contrato
- **Credor:** +[PONTO_SUCESSO_CREDOR] pontos
- **Devedor:** +[PONTO_SUCESSO_DEVEDOR] pontos
- **Árbitro:** +[PONTO_SUCESSO_ARBITRO] pontos (se envolvido)

### Falha do Contrato
- **Parte em falta:** -[PONTO_FALHA] pontos
- **Parte prejudicada:** +[PONTO_COMPENSACAO] pontos
- **Árbitro:** +[PONTO_DECISAO_JUSTA] pontos

### Uso do Seguro
- **Sinistro coberto:** Reputação mantida
- **Sinistro rejeitado:** -[PONTO_SINISTRO_REJEITADO] pontos
- **Fraude no sinistro:** -[PONTO_FRAUDE] pontos

## Riscos e Limitações

### Risco de Flutuação
- Flutuação de preço é risco mútuo
- Não sujeito a arbitragem
- Aceito por ambas as partes

### Limitações dos Redutores
- Reduções baseadas no momento da assinatura
- Mudanças durante o contrato não afetam benefícios
- Máximo de redução limitado a [PERCENTUAL_MAXIMO_REDUCAO]%

### Limitações do Seguro
- Cobertura limitada a [LIMITE_COBERTURA] BTC
- Não cobre flutuação de preço
- Sujeito a aprovação dos gestores

## Assinaturas Digitais

### Credor
- **Chave pública:** [CHAVE_CREDOR]
- **Reputação:** [REPUTACAO_CREDOR] pontos
- **Seguro:** [STATUS_SEGURO_CREDOR]
- **Assinatura:** [ASSINATURA_CREDOR]
- **Data:** [DATA_ASSINATURA_CREDOR]

### Devedor
- **Chave pública:** [CHAVE_DEVEDOR]
- **Reputação:** [REPUTACAO_DEVEDOR] pontos
- **Seguro:** [STATUS_SEGURO_DEVEDOR]
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

### Endereços
- **Multisig:** [ENDERECO_MULTISIG]
- **Fundo de Seguro:** [ENDERECO_FUNDO]
- **Associação:** [ENDERECO_ASSOCIACAO]

### Quorum
- **Multisig:** 2-de-3
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
- `[COLATERAL_FINAL_BTC]`: Colateral final em Bitcoin
- `[TAXA_JUROS]`: Taxa de juros mensal
- `[PRAZO_DIAS]`: Prazo em dias
- `[DATA_VENCIMENTO]`: Data de vencimento
- `[PERCENTUAL_REDUCAO_REPUTACAO]`: Redução por reputação
- `[PERCENTUAL_REDUCAO_SEGURO]`: Redução por seguro
- `[PERCENTUAL_REDUCAO_ASSOCIACAO]`: Redução por associação
- `[PERCENTUAL_REDUCAO_TOTAL]`: Redução total
- `[PERCENTUAL_MAXIMO_REDUCAO]`: Máximo de redução
- `[PLATAFORMA_WOT]`: Plataforma Web of Trust
- `[REPUTACAO_MINIMA]`: Reputação mínima necessária
- `[TAXA_SEGURO]`: Taxa do seguro
- `[LIMITE_COBERTURA]`: Limite de cobertura do seguro
- `[NOME_ASSOCIACAO]`: Nome da associação
- `[PLATAFORMA_COMUNICACAO]`: Plataforma de comunicação
- `[PLATAFORMA_ASSINATURA]`: Plataforma de assinatura
- `[PONTO_SUCESSO_CREDOR]`: Pontos por sucesso (credor)
- `[PONTO_SUCESSO_DEVEDOR]`: Pontos por sucesso (devedor)
- `[PONTO_SUCESSO_ARBITRO]`: Pontos por sucesso (árbitro)
- `[PONTO_FALHA]`: Pontos perdidos por falha
- `[PONTO_COMPENSACAO]`: Pontos por compensação
- `[PONTO_DECISAO_JUSTA]`: Pontos por decisão justa
- `[PONTO_SINISTRO_REJEITADO]`: Pontos perdidos por sinistro rejeitado
- `[PONTO_FRAUDE]`: Pontos perdidos por fraude
- `[STATUS_SEGURO_CREDOR]`: Status do seguro (credor)
- `[STATUS_SEGURO_DEVEDOR]`: Status do seguro (devedor)
- `[ASSINATURA_CREDOR]`: Assinatura digital do credor
- `[ASSINATURA_DEVEDOR]`: Assinatura digital do devedor
- `[ASSINATURA_ARBITRO]`: Assinatura digital do árbitro
- `[DATA_ASSINATURA_CREDOR]`: Data de assinatura do credor
- `[DATA_ASSINATURA_DEVEDOR]`: Data de assinatura do devedor
- `[DATA_ASSINATURA_ARBITRO]`: Data de assinatura do árbitro
- `[HASH_DOCUMENTO]`: Hash SHA256 do documento
- `[ENDERECO_MULTISIG]`: Endereço da multisig
- `[ENDERECO_FUNDO]`: Endereço do fundo de seguro
- `[ENDERECO_ASSOCIACAO]`: Endereço da associação
- `[TIMESTAMP_CRIACAO]`: Timestamp de criação
- `[TIMESTAMP_ASSINATURA]`: Timestamp de assinatura
- `[TIMESTAMP_VENCIMENTO]`: Timestamp de vencimento
