# Cláusulas de Reputação

## Cláusula Básica de Reputação

### 1. Sistema de Reputação

**1.1.** Este contrato utiliza o sistema Web of Trust (WoT) da Private Law Society para avaliação de reputação das partes.

**1.2.** A reputação será verificada através da plataforma [PLATAFORMA_REPUTACAO] no momento da assinatura do contrato.

**1.3.** Cada parte deve fornecer sua chave pública [CHAVE_PUBLICA] para verificação de reputação.

### 2. Pontuação de Reputação

**2.1.** A reputação é calculada com base em:
- a) Transações concluídas com sucesso: +[PONTO_SUCESSO] pontos
- b) Descumprimentos ou fraudes: -[PONTO_FALHA] pontos
- c) Recomendações de outros membros: +[PONTO_RECOMENDACAO] pontos
- d) Violações de contratos: -[PONTO_VIOLACAO] pontos

**2.2.** A reputação mínima para participação em contratos é [REPUTACAO_MINIMA] pontos.

**2.3.** A reputação será atualizada automaticamente após cada transação concluída.

## Cláusula de Benefícios por Reputação

### 3. Redução de Colateral

**3.1.** Partes com reputação acima de [LIMITE_REPUTACAO_ALTA] pontos terão benefícios especiais:
- a) Redução de colateral em [PERCENTUAL_REDUCAO]%
- b) Prioridade na escolha de árbitros
- c) Taxas reduzidas em fundos de seguro

**3.2.** Partes com reputação acima de [LIMITE_REPUTACAO_PREMIUM] pontos terão benefícios premium:
- a) Redução adicional de colateral em [PERCENTUAL_REDUCAO_PREMIUM]%
- b) Acesso a contratos de maior valor
- c) Desconto em taxas de arbitragem

### 4. Penalidades por Baixa Reputação

**4.1.** Partes com reputação abaixo de [LIMITE_REPUTACAO_BAIXA] pontos:
- a) Terão colateral aumentado em [PERCENTUAL_AUMENTO]%
- b) Serão limitadas a contratos de menor valor
- c) Poderão ser excluídas de novos contratos

**4.2.** Partes com reputação negativa (abaixo de 0) não poderão participar de novos contratos até recuperarem reputação positiva.

## Cláusula de Atualização de Reputação

### 5. Registro de Transações

**5.1.** Todas as transações devem ser registradas na plataforma [PLATAFORMA_REPUTACAO] com:
- a) Identificação das partes envolvidas
- b) Valor e tipo de transação
- c) Resultado (sucesso/falha)
- d) Evidências de cumprimento ou descumprimento

**5.2.** O registro deve ser feito em até [PRAZO_REGISTRO] dias após a conclusão da transação.

**5.3.** Evidências devem incluir:
- a) Comprovantes de pagamento
- b) Comunicações relevantes
- c) Decisões arbitrais, se aplicável

### 6. Avaliação de Reputação

**6.1.** A reputação será avaliada por:
- a) Sistema automatizado baseado em histórico
- b) Avaliações subjetivas de outros membros
- c) Decisões arbitrais em disputas

**6.2.** Disputas sobre reputação serão resolvidas por arbitragem conforme cláusulas de arbitragem deste contrato.

## Cláusula de Reputação para Árbitros

### 7. Reputação de Árbitros

**7.1.** Árbitros devem manter reputação mínima de [REPUTACAO_MINIMA_ARBITRO] pontos.

**7.2.** A reputação de árbitros é baseada em:
- a) Decisões justas e imparciais: +[PONTO_DECISAO_JUSTA] pontos
- b) Decisões tendenciosas: -[PONTO_DECISAO_TENDENCIOSA] pontos
- c) Tempo de resposta: +[PONTO_RAPIDEZ] pontos por decisão em prazo
- d) Disponibilidade: +[PONTO_DISPONIBILIDADE] pontos por aceitar casos

**7.3.** Árbitros com reputação abaixo de [REPUTACAO_MINIMA_ARBITRO] pontos serão removidos da lista de árbitros disponíveis.

## Cláusula de Transparência

### 8. Publicidade da Reputação

**8.1.** A reputação de cada parte será pública e verificável através da plataforma [PLATAFORMA_REPUTACAO].

**8.2.** Histórico de transações será mantido por [PRAZO_HISTORICO] anos para auditoria.

**8.3.** Partes podem contestar avaliações de reputação através de processo de arbitragem.

## Variáveis de Template

- `[PLATAFORMA_REPUTACAO]`: Plataforma de reputação (ex: Nostr WoT)
- `[CHAVE_PUBLICA]`: Chave pública da parte
- `[PONTO_SUCESSO]`: Pontos por transação bem-sucedida (ex: 5)
- `[PONTO_FALHA]`: Pontos perdidos por falha (ex: 10)
- `[PONTO_RECOMENDACAO]`: Pontos por recomendação (ex: 3)
- `[PONTO_VIOLACAO]`: Pontos perdidos por violação (ex: 15)
- `[REPUTACAO_MINIMA]`: Reputação mínima para contratos (ex: 10)
- `[LIMITE_REPUTACAO_ALTA]`: Limite para benefícios (ex: 50)
- `[LIMITE_REPUTACAO_PREMIUM]`: Limite para benefícios premium (ex: 100)
- `[LIMITE_REPUTACAO_BAIXA]`: Limite para penalidades (ex: 20)
- `[PERCENTUAL_REDUCAO]`: Redução de colateral (ex: 10%)
- `[PERCENTUAL_REDUCAO_PREMIUM]`: Redução premium (ex: 5%)
- `[PERCENTUAL_AUMENTO]`: Aumento de colateral (ex: 20%)
- `[PRAZO_REGISTRO]`: Prazo para registro (ex: 7 dias)
- `[REPUTACAO_MINIMA_ARBITRO]`: Reputação mínima para árbitros (ex: 75)
- `[PONTO_DECISAO_JUSTA]`: Pontos por decisão justa (ex: 5)
- `[PONTO_DECISAO_TENDENCIOSA]`: Pontos perdidos por decisão tendenciosa (ex: 20)
- `[PONTO_RAPIDEZ]`: Pontos por rapidez (ex: 2)
- `[PONTO_DISPONIBILIDADE]`: Pontos por disponibilidade (ex: 1)
- `[PRAZO_HISTORICO]`: Prazo de manutenção do histórico (ex: 5)
