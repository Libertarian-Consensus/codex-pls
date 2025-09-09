# Cláusulas de Seguro

## Cláusula Básica de Seguro

### 1. Fundo de Seguro Mútuo

**1.1.** Este contrato pode incluir cobertura do fundo de seguro mútuo da Private Law Society, operado através do endereço [ENDERECO_FUNDO].

**1.2.** A cobertura é opcional e deve ser solicitada no momento da assinatura do contrato.

**1.3.** O fundo de seguro é um mecanismo de proteção mútua, não uma seguradora regulamentada.

### 2. Condições de Cobertura

**2.1.** Para ter direito à cobertura, a parte deve:
- a) Ser membro ativo do fundo de seguro
- b) Ter contribuições em dia
- c) Não ter histórico de fraudes ou violações
- d) Seguir os procedimentos de sinistro

**2.2.** A cobertura se aplica a:
- a) Perdas por inadimplência da outra parte
- b) Perdas por falhas técnicas não culposas
- c) Custos de arbitragem em disputas válidas
- d) Perdas por violação contratual comprovada

**2.3.** A cobertura NÃO se aplica a:
- a) Flutuações de preço de Bitcoin
- b) Perdas por negligência própria
- c) Violações intencionais de contratos
- d) Perdas por eventos de força maior

## Cláusula de Contribuições

### 3. Taxas de Seguro

**3.1.** As contribuições para o fundo de seguro incluem:
- a) Taxa inicial de [TAXA_INICIAL] BTC
- b) Taxa mensal de [TAXA_MENSAL] BTC
- c) Taxa por contrato de [TAXA_CONTRATO]% do valor

**3.2.** As contribuições devem ser depositadas em:
- a) Taxa inicial: [ENDERECO_FUNDO]
- b) Taxa mensal: [ENDERECO_FUNDO]
- c) Taxa por contrato: [ENDERECO_FUNDO]

**3.3.** Contribuições em atraso resultam em suspensão da cobertura até regularização.

### 4. Gestão do Fundo

**4.1.** O fundo é gerenciado por [NUMERO_GESTORES] gestores eleitos pelos participantes.

**4.2.** As chaves do fundo são mantidas em multisig [QUORUM_FUNDO]-de-[TOTAL_FUNDO] por:
- a) [NUMERO_GESTORES] gestores eleitos pelos participantes
- b) [NUMERO_ARBITROS_FUNDO] árbitros escolhidos pelos participantes
- c) Representante da associação (se aplicável)

**4.3.** Decisões sobre o fundo requerem [PERCENTUAL_APROVACAO_FUNDO]% de aprovação dos gestores.

## Cláusula de Sinistros

### 5. Processo de Sinistro

**5.1.** Para solicitar cobertura de sinistro, a parte deve:
- a) Notificar o fundo em até [PRAZO_NOTIFICACAO] dias após o evento
- b) Apresentar evidências detalhadas da perda
- c) Demonstrar que seguiu os procedimentos contratuais
- d) Aceitar investigação e arbitragem se necessário

**5.2.** A documentação deve incluir:
- a) Contrato original assinado
- b) Evidências da violação ou perda
- c) Tentativas de resolução amigável
- d) Decisão arbitral (se aplicável)

### 6. Limites de Cobertura

**6.1.** Os limites de cobertura são:
- a) Máximo por sinistro: [LIMITE_SINISTRO] BTC
- b) Máximo anual por participante: [LIMITE_ANUAL] BTC
- c) Máximo total do fundo: [LIMITE_FUNDO] BTC

**6.2.** Em caso de múltiplos sinistros simultâneos, a cobertura será distribuída proporcionalmente.

**6.3.** Sinistros acima dos limites serão cobertos parcialmente ou rejeitados.

## Cláusula de Redução de Colateral

### 7. Benefício de Redução

**7.1.** Participantes do fundo de seguro têm direito a redução de colateral de [PERCENTUAL_REDUCAO]%.

**7.2.** A redução se aplica a:
- a) Contratos entre participantes do fundo
- b) Contratos com participantes de alta reputação
- c) Contratos de valor até [VALOR_MAXIMO_REDUCAO] BTC

**7.3.** A redução é calculada como:
```
Colateral Final = Colateral Base × (1 - Percentual_Redução_Seguro)
```

### 8. Condições para Redução

**8.1.** A redução de colateral está sujeita a:
- a) Participação ativa no fundo de seguro
- b) Contribuições em dia
- c) Reputação mínima de [REPUTACAO_MINIMA_SEGURO] pontos
- d) Aprovação pelos gestores do fundo

**8.2.** A redução pode ser revogada se:
- a) Contribuições ficarem em atraso
- b) Reputação cair abaixo do mínimo
- c) Houver violação dos termos do fundo

## Cláusula de Exclusão e Cancelamento

### 9. Exclusão do Fundo

**9.1.** Um participante pode ser excluído do fundo por:
- a) Fraude ou violação intencional
- b) Múltiplos sinistros sem justificativa
- c) Não pagamento de contribuições
- d) Decisão arbitral de exclusão

**9.2.** A exclusão resulta em:
- a) Perda de cobertura imediata
- b) Perda de benefícios de redução de colateral
- c) Não reembolso de contribuições pagas
- d) Possível penalização de reputação

### 10. Saída Voluntária

**10.1.** Participantes podem sair voluntariamente do fundo com:
- a) Notificação prévia de [PRAZO_SAIDA] dias
- b) Quitação de pendências
- c) Não reembolso de contribuições

**10.2.** A saída voluntária não afeta contratos já em vigor.

## Variáveis de Template

- `[ENDERECO_FUNDO]`: Endereço da carteira do fundo de seguro
- `[TAXA_INICIAL]`: Taxa inicial em BTC (ex: 0.005)
- `[TAXA_MENSAL]`: Taxa mensal em BTC (ex: 0.001)
- `[TAXA_CONTRATO]`: Taxa por contrato em % (ex: 1%)
- `[NUMERO_GESTORES]`: Número de gestores do fundo (ex: 5)
- `[QUORUM_FUNDO]`: Quorum para multisig do fundo (ex: 3)
- `[TOTAL_FUNDO]`: Total de chaves do fundo (ex: 7)
- `[NUMERO_ARBITROS_FUNDO]`: Número de árbitros do fundo (ex: 2)
- `[PERCENTUAL_APROVACAO_FUNDO]`: % para aprovação (ex: 75%)
- `[PRAZO_NOTIFICACAO]`: Prazo para notificar sinistro (ex: 7 dias)
- `[LIMITE_SINISTRO]`: Limite por sinistro em BTC (ex: 0.05)
- `[LIMITE_ANUAL]`: Limite anual por participante em BTC (ex: 0.2)
- `[LIMITE_FUNDO]`: Limite total do fundo em BTC (ex: 1.0)
- `[PERCENTUAL_REDUCAO]`: Redução de colateral em % (ex: 15%)
- `[VALOR_MAXIMO_REDUCAO]`: Valor máximo para redução em BTC (ex: 0.5)
- `[REPUTACAO_MINIMA_SEGURO]`: Reputação mínima para seguro (ex: 30)
- `[PRAZO_SAIDA]`: Prazo para saída voluntária (ex: 30 dias)
