# Cláusulas de Arbitragem

## Cláusula Básica de Arbitragem

### 1. Escolha de Árbitro

**1.1.** As partes concordam em escolher [NOME_ARBITRO] como árbitro para resolução de disputas relacionadas a este contrato.

**1.2.** O árbitro deve:
- a) Ser escolhido por consenso entre as partes
- b) Manter reputação mínima de [REPUTACAO_MINIMA_ARBITRO] pontos (se aplicável)
- c) Não ter conflito de interesses com as partes
- d) Aceitar a jurisdição deste contrato

**1.3.** Em caso de indisponibilidade do árbitro escolhido, as partes podem:
- a) Escolher um árbitro substituto por consenso
- b) Consultar listas públicas de árbitros disponíveis
- c) Usar o árbitro com maior reputação disponível (se aplicável)

### 2. Jurisdição do Árbitro

**2.1.** O árbitro terá jurisdição para decidir sobre:
- a) Cumprimento ou descumprimento de obrigações contratuais
- b) Interpretação de cláusulas contratuais
- c) Validação de evidências apresentadas
- d) Aplicação de penalidades e multas

**2.2.** O árbitro NÃO terá jurisdição sobre:
- a) Flutuações de preço de Bitcoin ou outras criptomoedas
- b) Questões de direito estatal ou regulamentações governamentais
- c) Disputas não relacionadas a este contrato específico

## Cláusula de Processo Arbitral

### 3. Iniciação de Disputa

**3.1.** Qualquer parte pode iniciar uma disputa notificando:
- a) A outra parte via meio acordado (email, mensagem direta, etc.)
- b) O árbitro escolhido
- c) O sistema de reputação (se aplicável)

**3.2.** A notificação deve incluir:
- a) Descrição detalhada da disputa
- b) Evidências relevantes
- c) Solicitação específica de resolução
- d) Prazo para resposta da outra parte

### 4. Apresentação de Evidências

**4.1.** Cada parte terá [PRAZO_EVIDENCIA] dias para apresentar evidências após a notificação de disputa.

**4.2.** Evidências aceitas incluem:
- a) Comunicações registradas na plataforma
- b) Comprovantes de pagamento ou transação
- c) Testemunhos de terceiros
- d) Documentos assinados digitalmente

**4.3.** Evidências devem ser apresentadas via meio acordado com timestamp verificável.

### 5. Decisão Arbitral

**5.1.** O árbitro deve emitir decisão em até [PRAZO_DECISAO] dias após recebimento de todas as evidências.

**5.2.** A decisão deve incluir:
- a) Análise dos fatos apresentados
- b) Aplicação das cláusulas contratuais
- c) Decisão específica e executável
- d) Justificativa da decisão

**5.3.** A decisão será final e vinculante para ambas as partes.

## Cláusula de Execução da Decisão

### 6. Execução Automática

**6.1.** Decisões arbitrais serão executadas automaticamente através de:
- a) Liberação ou retenção de colateral
- b) Transferência de fundos via multisig
- c) Atualização de reputação no sistema WoT
- d) Aplicação de penalidades contratuais

**6.2.** A execução ocorrerá em até [PRAZO_EXECUCAO] dias após a decisão arbitral.

### 7. Recursos e Revisão

**7.1.** Em casos excepcionais, as partes podem solicitar revisão da decisão se:
- a) Houver evidência de parcialidade do árbitro
- b) Novas evidências relevantes forem descobertas
- c) Houver erro claro na aplicação das cláusulas

**7.2.** A revisão será conduzida por um painel de 3 árbitros de maior reputação disponíveis.

## Cláusula de Custos Arbitrais

### 8. Taxas de Arbitragem

**8.1.** As taxas de arbitragem serão:
- a) [TAXA_ARBITRAGEM]% do valor em disputa (mínimo [TAXA_MINIMA] BTC)
- b) Divididas igualmente entre as partes
- c) Deduzidas do colateral antes da execução da decisão

**8.2.** A parte vencedora pode solicitar reembolso das taxas pagas.

**8.3.** Em caso de disputa frívola, a parte responsável pagará todas as taxas.

## Cláusula de Múltiplos Árbitros

### 9. Arbitragem por Painel

**9.1.** Para contratos de alto valor (acima de [VALOR_ALTO]), as partes podem optar por painel de [NUMERO_ARBITROS] árbitros.

**9.2.** O painel será composto por:
- a) Um árbitro escolhido por cada parte
- b) Um árbitro presidente escolhido por consenso entre as partes
- c) Árbitros de maior reputação disponível (se aplicável)

**9.3.** Decisões do painel requerem maioria simples dos árbitros.

## Cláusula de Arbitragem de Emergência

### 10. Medidas Cautelares

**10.1.** Em casos de urgência, as partes podem solicitar medidas cautelares:
- a) Congelamento temporário de colateral
- b) Suspensão de execução de cláusulas
- c) Preservação de evidências

**10.2.** Medidas cautelares serão decididas em até [PRAZO_CAUTELAR] horas.

**10.3.** Medidas cautelares são temporárias e sujeitas a revisão no processo arbitral principal.

## Variáveis de Template

- `[NOME_ARBITRO]`: Nome ou identificador do árbitro
- `[REPUTACAO_MINIMA_ARBITRO]`: Reputação mínima para árbitros (ex: 75)
- `[PLATAFORMA_COMUNICACAO]`: Plataforma de comunicação (ex: Nostr)
- `[PRAZO_EVIDENCIA]`: Prazo para apresentar evidências (ex: 7 dias)
- `[PRAZO_DECISAO]`: Prazo para decisão (ex: 14 dias)
- `[PRAZO_EXECUCAO]`: Prazo para execução (ex: 3 dias)
- `[TAXA_ARBITRAGEM]`: Taxa de arbitragem (ex: 2%)
- `[TAXA_MINIMA]`: Taxa mínima em BTC (ex: 0.001)
- `[VALOR_ALTO]`: Valor para painel múltiplo (ex: 1.0 BTC)
- `[NUMERO_ARBITROS]`: Número de árbitros no painel (ex: 3)
- `[PRAZO_CAUTELAR]`: Prazo para medidas cautelares (ex: 24)
