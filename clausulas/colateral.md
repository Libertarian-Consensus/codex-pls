# Cláusulas de Colateral

## Cláusula Básica de Colateral

### 1. Depósito de Colateral

**1.1.** O [PARTE_DEVEDORA] depositará [VALOR_COLATERAL] BTC como colateral em uma carteira multisig [QUORUM]-de-[TOTAL], no endereço [ENDERECO_MULTISIG], válido por todo o período de vigência do contrato.

**1.2.** As chaves da carteira multisig serão mantidas por:
- a) [PARTE_DEVEDORA]: [CHAVE_DEVEDOR]
- b) [PARTE_CREDORA]: [CHAVE_CREDOR]  
- c) Árbitro: [CHAVE_ARBITRO]

**1.3.** O colateral será devolvido ao [PARTE_DEVEDORA] ao final do contrato, desde que todas as obrigações sejam cumpridas sem incidentes.

### 2. Liberação de Colateral

**2.1.** O colateral será liberado automaticamente quando:
- a) Ambas as partes concordarem com a liberação
- b) Uma das partes + quorum de árbitros concordarem
- c) O contrato for cumprido integralmente

**2.2.** O colateral pode ser retido em caso de:
- a) Inadimplência comprovada
- b) Violação dos termos contratuais
- c) Decisão arbitral favorável à retenção

## Cláusula de Colateral Ajustado por Reputação

### 3. Redução por Reputação

**3.1.** Membros com reputação acima de [LIMITE_REPUTACAO_ALTA] pontos no sistema WoT terão o colateral reduzido em [PERCENTUAL_REPUTACAO]%.

**3.2.** A reputação será verificada no momento da assinatura do contrato através da plataforma [PLATAFORMA_REPUTACAO].

**3.3.** O colateral ajustado será calculado como:
```
Colateral Final = Colateral Base × (1 - Percentual_Redução_Reputação)
```

## Cláusula de Colateral Ajustado por Seguro

### 4. Redução por Seguro

**4.1.** Participantes do fundo de seguro podem reduzir o colateral em [PERCENTUAL_SEGURO]%, mediante pagamento de taxa de [TAXA_SEGURO]% sobre o valor do contrato.

**4.2.** A taxa de seguro será depositada no endereço [ENDERECO_FUNDO] no início do contrato.

**4.3.** O colateral ajustado será calculado como:
```
Colateral Final = Colateral Base × (1 - Percentual_Redução_Seguro)
```

## Cláusula de Colateral Híbrido

### 5. Múltiplas Reduções

**5.1.** Quando aplicáveis, as reduções por reputação e seguro são cumulativas, limitadas a um máximo de [PERCENTUAL_MAXIMO_REDUCAO]%.

**5.2.** O colateral final será calculado como:
```
Colateral Final = Colateral Base × (1 - min(Redução_Reputação + Redução_Seguro, Percentual_Máximo))
```

**5.3.** O colateral mínimo será sempre [COLATERAL_MINIMO] BTC, independente das reduções aplicadas.

## Cláusula de Flutuação de Preço

### 6. Risco de Flutuação

**6.1.** Ambas as partes reconhecem que a flutuação de preço do Bitcoin é um risco mútuo e não será objeto de disputa ou arbitragem.

**6.2.** O valor do colateral será fixado no momento da assinatura do contrato e não será ajustado por flutuações de preço.

**6.3.** Em caso de disputa relacionada a flutuação de preço, o árbitro não terá jurisdição para decidir sobre o assunto.

## Variáveis de Template

- `[PARTE_DEVEDORA]`: Nome ou identificador da parte que deposita o colateral
- `[PARTE_CREDORA]`: Nome ou identificador da parte credora
- `[VALOR_COLATERAL]`: Valor em BTC do colateral
- `[QUORUM]`: Número mínimo de assinaturas necessárias (ex: 2)
- `[TOTAL]`: Número total de chaves na multisig (ex: 3)
- `[ENDERECO_MULTISIG]`: Endereço da carteira multisig
- `[CHAVE_DEVEDOR]`: Chave pública do devedor
- `[CHAVE_CREDOR]`: Chave pública do credor
- `[CHAVE_ARBITRO]`: Chave pública do árbitro
- `[LIMITE_REPUTACAO_ALTA]`: Pontuação mínima para redução (ex: 50)
- `[PERCENTUAL_REPUTACAO]`: Percentual de redução por reputação (ex: 10%)
- `[PLATAFORMA_REPUTACAO]`: Plataforma de verificação (ex: Nostr WoT)
- `[PERCENTUAL_SEGURO]`: Percentual de redução por seguro (ex: 15%)
- `[TAXA_SEGURO]`: Taxa do seguro (ex: 1%)
- `[ENDERECO_FUNDO]`: Endereço do fundo de seguro
- `[PERCENTUAL_MAXIMO_REDUCAO]`: Máximo de redução total (ex: 25%)
- `[COLATERAL_MINIMO]`: Colateral mínimo em BTC (ex: 0.001)
