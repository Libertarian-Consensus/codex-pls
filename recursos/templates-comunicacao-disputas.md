# Templates de Comunicação para Disputas

## Template de Notificação de Disputa

### Email/Comunicação Direta
```
Assunto: [DISPUTA] Contrato [ID_CONTRATO] - [TIPO_DISPUTA]

Para: [PARTE_RESPONDENTE], [ARBITRO]
De: [PARTE_REQUERENTE]
Data: [DATA_NOTIFICACAO]

Prezados,

Venho por meio desta notificar o início de uma disputa relacionada ao contrato [ID_CONTRATO], conforme especificado abaixo:

**Detalhes da Disputa:**
- Tipo: [TIPO_DISPUTA]
- Valor em disputa: [VALOR_DISPUTA] [MOEDA]
- Data do evento: [DATA_EVENTO]
- Descrição: [DESCRICAO_DETALHADA]

**Evidências Anexadas:**
- [EVIDENCIA_1]: [DESCRICAO_EVIDENCIA_1]
- [EVIDENCIA_2]: [DESCRICAO_EVIDENCIA_2]
- [EVIDENCIA_3]: [DESCRICAO_EVIDENCIA_3]

**Solicitação:**
[SOLICITACAO_ESPECIFICA]

**Prazo para Resposta:**
[PRAZO_RESPOSTA] dias a partir desta notificação.

**Árbitro Designado:**
[NOME_ARBITRO] - [CHAVE_PUBLICA_ARBITRO]

Atenciosamente,
[PARTE_REQUERENTE]
[CHAVE_PUBLICA_REQUERENTE]
[ASSINATURA_DIGITAL]
```

### Formato JSON (para sistemas automatizados)
```json
{
  "type": "dispute_notification",
  "version": "1.0",
  "contract_id": "[ID_CONTRATO]",
  "dispute_id": "[ID_DISPUTA]",
  "timestamp": [TIMESTAMP],
  "parties": {
    "requester": {
      "name": "[NOME_REQUERENTE]",
      "public_key": "[CHAVE_PUBLICA_REQUERENTE]"
    },
    "respondent": {
      "name": "[NOME_RESPONDENTE]",
      "public_key": "[CHAVE_PUBLICA_RESPONDENTE]"
    }
  },
  "arbitrator": {
    "name": "[NOME_ARBITRO]",
    "public_key": "[CHAVE_PUBLICA_ARBITRO]"
  },
  "dispute": {
    "type": "[TIPO_DISPUTA]",
    "value": "[VALOR_DISPUTA]",
    "currency": "[MOEDA]",
    "event_date": "[DATA_EVENTO]",
    "description": "[DESCRICAO_DETALHADA]",
    "request": "[SOLICITACAO_ESPECIFICA]"
  },
  "evidence": [
    {
      "id": "[EVIDENCIA_1]",
      "type": "[TIPO_EVIDENCIA_1]",
      "description": "[DESCRICAO_EVIDENCIA_1]",
      "hash": "[HASH_EVIDENCIA_1]"
    },
    {
      "id": "[EVIDENCIA_2]",
      "type": "[TIPO_EVIDENCIA_2]",
      "description": "[DESCRICAO_EVIDENCIA_2]",
      "hash": "[HASH_EVIDENCIA_2]"
    }
  ],
  "deadlines": {
    "response": "[PRAZO_RESPOSTA]",
    "evidence": "[PRAZO_EVIDENCIA]",
    "decision": "[PRAZO_DECISAO]"
  },
  "signature": "[ASSINATURA_DIGITAL]"
}
```

## Template de Resposta à Disputa

### Email/Comunicação Direta
```
Assunto: [RESPOSTA] Disputa [ID_DISPUTA] - Contrato [ID_CONTRATO]

Para: [PARTE_REQUERENTE], [ARBITRO]
De: [PARTE_RESPONDENTE]
Data: [DATA_RESPOSTA]

Prezados,

Venho por meio desta responder à disputa [ID_DISPUTA] relacionada ao contrato [ID_CONTRATO]:

**Posição da Parte:**
[POSICAO_DETALHADA]

**Contestação:**
[CONTESTACAO_ESPECIFICA]

**Evidências de Defesa:**
- [EVIDENCIA_DEFESA_1]: [DESCRICAO_EVIDENCIA_DEFESA_1]
- [EVIDENCIA_DEFESA_2]: [DESCRICAO_EVIDENCIA_DEFESA_2]
- [EVIDENCIA_DEFESA_3]: [DESCRICAO_EVIDENCIA_DEFESA_3]

**Contraproposta:**
[CONTRAPROPOSTA_ESPECIFICA]

**Solicitação de Evidências Adicionais:**
[SOLICITACAO_EVIDENCIAS_ADICIONAIS]

Atenciosamente,
[PARTE_RESPONDENTE]
[CHAVE_PUBLICA_RESPONDENTE]
[ASSINATURA_DIGITAL]
```

## Template de Decisão Arbitral

### Email/Comunicação Direta
```
Assunto: [DECISÃO] Disputa [ID_DISPUTA] - Contrato [ID_CONTRATO]

Para: [PARTE_REQUERENTE], [PARTE_RESPONDENTE]
De: [ARBITRO]
Data: [DATA_DECISAO]

Prezados,

Venho por meio desta comunicar a decisão arbitral referente à disputa [ID_DISPUTA]:

**Resumo da Disputa:**
[RESUMO_DISPUTA]

**Análise das Evidências:**
[ANALISE_EVIDENCIAS]

**Aplicação das Cláusulas Contratuais:**
[APLICACAO_CLÁUSULAS]

**Decisão:**
[DECISAO_ESPECIFICA]

**Justificativa:**
[JUSTIFICATIVA_DETALHADA]

**Valor da Indenização:**
[VALOR_INDENIZACAO] [MOEDA]

**Prazo para Execução:**
[PRAZO_EXECUCAO] dias

**Recursos:**
[INFORMACOES_RECURSOS]

Esta decisão é final e vinculante para ambas as partes.

Atenciosamente,
[ARBITRO]
[CHAVE_PUBLICA_ARBITRO]
[ASSINATURA_DIGITAL]
```

### Formato JSON (para sistemas automatizados)
```json
{
  "type": "arbitral_decision",
  "version": "1.0",
  "dispute_id": "[ID_DISPUTA]",
  "contract_id": "[ID_CONTRATO]",
  "timestamp": [TIMESTAMP],
  "arbitrator": {
    "name": "[NOME_ARBITRO]",
    "public_key": "[CHAVE_PUBLICA_ARBITRO]"
  },
  "decision": {
    "summary": "[RESUMO_DISPUTA]",
    "analysis": "[ANALISE_EVIDENCIAS]",
    "application": "[APLICACAO_CLÁUSULAS]",
    "ruling": "[DECISAO_ESPECIFICA]",
    "reasoning": "[JUSTIFICATIVA_DETALHADA]",
    "award": {
      "value": "[VALOR_INDENIZACAO]",
      "currency": "[MOEDA]"
    },
    "execution_deadline": "[PRAZO_EXECUCAO]"
  },
  "appeals": {
    "available": [DISPONIVEL_RECURSO],
    "deadline": "[PRAZO_RECURSO]",
    "procedure": "[PROCEDIMENTO_RECURSO]"
  },
  "signature": "[ASSINATURA_DIGITAL]"
}
```

## Template de Evidência

### Formato JSON
```json
{
  "type": "evidence",
  "version": "1.0",
  "evidence_id": "[ID_EVIDENCIA]",
  "dispute_id": "[ID_DISPUTA]",
  "contract_id": "[ID_CONTRATO]",
  "timestamp": [TIMESTAMP],
  "submitter": {
    "name": "[NOME_SUBMISSOR]",
    "public_key": "[CHAVE_PUBLICA_SUBMISSOR]"
  },
  "evidence": {
    "type": "[TIPO_EVIDENCIA]",
    "description": "[DESCRICAO_EVIDENCIA]",
    "content": "[CONTEUDO_OU_HASH]",
    "format": "[FORMATO_ARQUIVO]",
    "size": "[TAMANHO_ARQUIVO]",
    "hash": "[HASH_EVIDENCIA]"
  },
  "metadata": {
    "created_date": "[DATA_CRIACAO]",
    "source": "[FONTE_EVIDENCIA]",
    "authenticity": "[VERIFICACAO_AUTENTICIDADE]"
  },
  "signature": "[ASSINATURA_DIGITAL]"
}
```

## Template de Notificação de Execução

### Email/Comunicação Direta
```
Assunto: [EXECUÇÃO] Decisão [ID_DISPUTA] - Contrato [ID_CONTRATO]

Para: [PARTE_REQUERENTE], [PARTE_RESPONDENTE]
De: [ARBITRO]
Data: [DATA_EXECUCAO]

Prezados,

Venho por meio desta comunicar a execução da decisão arbitral [ID_DISPUTA]:

**Status da Execução:**
[STATUS_EXECUCAO]

**Ações Tomadas:**
[ACOES_TOMADAS]

**Valor Transferido:**
[VALOR_TRANSFERIDO] [MOEDA]

**Endereço de Destino:**
[ENDERECO_DESTINO]

**Hash da Transação:**
[HASH_TRANSACAO]

**Comprovante:**
[COMPROVANTE_EXECUCAO]

A execução foi concluída conforme decisão arbitral.

Atenciosamente,
[ARBITRO]
[CHAVE_PUBLICA_ARBITRO]
[ASSINATURA_DIGITAL]
```

## Variáveis de Template

### Identificadores
- `[ID_CONTRATO]`: Identificador único do contrato
- `[ID_DISPUTA]`: Identificador único da disputa
- `[ID_EVIDENCIA]`: Identificador único da evidência

### Partes
- `[NOME_REQUERENTE]`: Nome da parte que inicia a disputa
- `[NOME_RESPONDENTE]`: Nome da parte que responde à disputa
- `[NOME_ARBITRO]`: Nome do árbitro
- `[CHAVE_PUBLICA_REQUERENTE]`: Chave pública do requerente
- `[CHAVE_PUBLICA_RESPONDENTE]`: Chave pública do respondente
- `[CHAVE_PUBLICA_ARBITRO]`: Chave pública do árbitro

### Disputa
- `[TIPO_DISPUTA]`: Tipo da disputa (inadimplência, violação, etc.)
- `[VALOR_DISPUTA]`: Valor em disputa
- `[MOEDA]`: Moeda da disputa
- `[DATA_EVENTO]`: Data do evento que gerou a disputa
- `[DESCRICAO_DETALHADA]`: Descrição detalhada da disputa
- `[SOLICITACAO_ESPECIFICA]`: Solicitação específica

### Prazos
- `[PRAZO_RESPOSTA]`: Prazo para resposta em dias
- `[PRAZO_EVIDENCIA]`: Prazo para apresentar evidências
- `[PRAZO_DECISAO]`: Prazo para decisão arbitral
- `[PRAZO_EXECUCAO]`: Prazo para execução da decisão

### Evidências
- `[EVIDENCIA_1]`: Identificador da primeira evidência
- `[TIPO_EVIDENCIA_1]`: Tipo da primeira evidência
- `[DESCRICAO_EVIDENCIA_1]`: Descrição da primeira evidência
- `[HASH_EVIDENCIA_1]`: Hash da primeira evidência

### Decisão
- `[RESUMO_DISPUTA]`: Resumo da disputa
- `[ANALISE_EVIDENCIAS]`: Análise das evidências
- `[APLICACAO_CLÁUSULAS]`: Aplicação das cláusulas contratuais
- `[DECISAO_ESPECIFICA]`: Decisão específica
- `[JUSTIFICATIVA_DETALHADA]`: Justificativa detalhada
- `[VALOR_INDENIZACAO]`: Valor da indenização

### Execução
- `[STATUS_EXECUCAO]`: Status da execução
- `[ACOES_TOMADAS]`: Ações tomadas
- `[VALOR_TRANSFERIDO]`: Valor transferido
- `[ENDERECO_DESTINO]`: Endereço de destino
- `[HASH_TRANSACAO]`: Hash da transação
- `[COMPROVANTE_EXECUCAO]`: Comprovante da execução

### Assinaturas
- `[ASSINATURA_DIGITAL]`: Assinatura digital
- `[TIMESTAMP]`: Timestamp Unix
- `[DATA_NOTIFICACAO]`: Data da notificação
- `[DATA_RESPOSTA]`: Data da resposta
- `[DATA_DECISAO]`: Data da decisão
- `[DATA_EXECUCAO]`: Data da execução
