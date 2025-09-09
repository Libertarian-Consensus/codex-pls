# Contrato de Seguro Básico

**Versão:** 1.0  
**Data:** [DATA_CONTRATO]  
**Protocolo:** PLS (PLIP-01)

## Partes

- **Participante:** [NOME_PARTICIPANTE], chave pública: [CHAVE_PARTICIPANTE]
- **Gestor do Fundo:** [NOME_GESTOR], chave pública: [CHAVE_GESTOR]
- **Árbitro:** [NOME_ARBITRO], chave pública: [CHAVE_ARBITRO]

## Objetivo

Este contrato estabelece os termos para participação no fundo de seguro básico, oferecendo proteção contra perdas em transações e disputas.

## Termos do Seguro

### 1. Cobertura
- **Tipo**: Seguro básico contra inadimplência
- **Limite**: [LIMITE_COBERTURA] BTC por sinistro
- **Período**: [PERIODO_COBERTURA] dias
- **Renovação**: Automática se contribuições estiverem em dia

### 2. Contribuições
- **Taxa Inicial**: [TAXA_INICIAL] BTC
- **Taxa Mensal**: [TAXA_MENSAL] BTC
- **Taxa por Contrato**: [TAXA_CONTRATO]% do valor
- **Endereço do Fundo**: [ENDERECO_FUNDO]

### 3. Elegibilidade
- **Membro Ativo**: Deve ser membro ativo da associação
- **Reputação Mínima**: [REPUTACAO_MINIMA] pontos
- **Contribuições em Dia**: Sem atrasos nas contribuições
- **Sem Violações**: Sem violações recentes

## Cláusulas Modulares

### Cláusula de Colateral
*[Incluir cláusula de colateral básica - ver [clausulas/colateral.md](../../clausulas/colateral.md)]*

**Colateral:** [COLATERAL_SEGURO] BTC depositado em multisig 2-de-3

### Cláusula de Seguro
*[Incluir cláusula de seguro básica - ver [clausulas/seguro.md](../../clausulas/seguro.md)]*

**Cobertura:** [LIMITE_COBERTURA] BTC com taxa de [TAXA_CONTRATO]%

### Cláusula de Arbitragem
*[Incluir cláusula de arbitragem básica - ver [clausulas/arbitragem.md](../../clausulas/arbitragem.md)]*

**Árbitro:** [NOME_ARBITRO] para disputas sobre cobertura

### Cláusula de Comunicação
*[Incluir cláusula de comunicação básica - ver [clausulas/comunicacao.md](../../clausulas/comunicacao.md)]*

**Plataforma:** [PLATAFORMA_COMUNICACAO] para notificações

## Processo de Sinistro

### 1. Notificação
- **Prazo**: 7 dias após o evento
- **Método**: [PLATAFORMA_COMUNICACAO]
- **Documentação**: Evidências detalhadas
- **Valor**: Valor específico da perda

### 2. Investigação
- **Prazo**: 14 dias para investigação
- **Responsável**: Gestor do fundo
- **Critérios**: Verificação de elegibilidade
- **Decisão**: Aprovação ou rejeição

### 3. Pagamento
- **Prazo**: 7 dias após aprovação
- **Método**: Transferência Bitcoin
- **Valor**: Valor aprovado (até limite)
- **Comprovante**: Hash da transação

## Exclusões

### 1. Não Coberto
- **Flutuação de Preço**: Variações de preço do Bitcoin
- **Negligência Própria**: Perdas por negligência do participante
- **Violações Intencionais**: Violações intencionais de contratos
- **Força Maior**: Eventos fora de controle

### 2. Limitações
- **Limite por Sinistro**: [LIMITE_COBERTURA] BTC
- **Limite Anual**: [LIMITE_ANUAL] BTC
- **Período de Carência**: [PERIODO_CARENCIA] dias
- **Exclusões Específicas**: Conforme definido no contrato

## Gestão do Fundo

### 1. Estrutura
- **Gestor Principal**: [NOME_GESTOR]
- **Árbitros**: [NUMERO_ARBITROS] árbitros de confiança
- **Multisig**: [QUORUM]-de-[TOTAL] para liberação
- **Auditoria**: Auditoria trimestral

### 2. Decisões
- **Aprovação de Sinistros**: [PERCENTUAL_APROVACAO]% dos gestores
- **Alterações de Regras**: [PERCENTUAL_ALTERACAO]% dos participantes
- **Dissolução**: [PERCENTUAL_DISSOLUCAO]% dos participantes
- **Emergência**: Decisões de emergência por gestor

### 3. Transparência
- **Relatórios**: Relatórios mensais públicos
- **Auditoria**: Auditoria independente
- **Comunicação**: Comunicação regular com participantes
- **Feedback**: Sistema de feedback dos participantes

## Cancelamento e Saída

### 1. Cancelamento pelo Participante
- **Notificação**: 30 dias de antecedência
- **Motivo**: Qualquer motivo
- **Reembolso**: Sem reembolso de contribuições
- **Cobertura**: Cobertura mantida até fim do período

### 2. Cancelamento pelo Fundo
- **Motivos**: Violação de termos, fraude, inadimplência
- **Processo**: Notificação + prazo para correção
- **Efeito**: Perda de cobertura imediata
- **Reembolso**: Sem reembolso de contribuições

### 3. Dissolução do Fundo
- **Decisão**: [PERCENTUAL_DISSOLUCAO]% dos participantes
- **Processo**: Votação + notificação
- **Distribuição**: Distribuição proporcional dos fundos
- **Prazo**: 90 dias para distribuição

## Assinaturas Digitais

### Participante
- **Chave pública:** [CHAVE_PARTICIPANTE]
- **Assinatura:** [ASSINATURA_PARTICIPANTE]
- **Data:** [DATA_ASSINATURA_PARTICIPANTE]

### Gestor do Fundo
- **Chave pública:** [CHAVE_GESTOR]
- **Assinatura:** [ASSINATURA_GESTOR]
- **Data:** [DATA_ASSINATURA_GESTOR]

### Árbitro
- **Chave pública:** [CHAVE_ARBITRO]
- **Assinatura:** [ASSINATURA_ARBITRO]
- **Data:** [DATA_ASSINATURA_ARBITRO]

## Metadados do Contrato

### Hash do Documento
- **SHA256:** [HASH_DOCUMENTO]

### Endereços
- **Multisig:** [ENDERECO_MULTISIG]
- **Fundo:** [ENDERECO_FUNDO]

### Quorum
- **Multisig:** 2-de-3
- **Chaves:** [CHAVE_PARTICIPANTE], [CHAVE_GESTOR], [CHAVE_ARBITRO]

### Timestamps
- **Criado:** [TIMESTAMP_CRIACAO]
- **Assinado:** [TIMESTAMP_ASSINATURA]
- **Vigência:** [TIMESTAMP_VIGENCIA]

## Variáveis de Template

- `[DATA_CONTRATO]`: Data de criação do contrato
- `[NOME_PARTICIPANTE]`: Nome ou pseudônimo do participante
- `[NOME_GESTOR]`: Nome ou pseudônimo do gestor
- `[NOME_ARBITRO]`: Nome ou pseudônimo do árbitro
- `[CHAVE_PARTICIPANTE]`: Chave pública do participante
- `[CHAVE_GESTOR]`: Chave pública do gestor
- `[CHAVE_ARBITRO]`: Chave pública do árbitro
- `[LIMITE_COBERTURA]`: Limite de cobertura em BTC
- `[PERIODO_COBERTURA]`: Período de cobertura em dias
- `[TAXA_INICIAL]`: Taxa inicial em BTC
- `[TAXA_MENSAL]`: Taxa mensal em BTC
- `[TAXA_CONTRATO]`: Taxa por contrato em %
- `[ENDERECO_FUNDO]`: Endereço do fundo
- `[REPUTACAO_MINIMA]`: Reputação mínima necessária
- `[COLATERAL_SEGURO]`: Colateral do seguro em BTC
- `[LIMITE_ANUAL]`: Limite anual em BTC
- `[PERIODO_CARENCIA]`: Período de carência em dias
- `[NUMERO_ARBITROS]`: Número de árbitros
- `[QUORUM]`: Quorum para multisig
- `[TOTAL]`: Total de chaves para multisig
- `[PERCENTUAL_APROVACAO]`: Percentual para aprovação
- `[PERCENTUAL_ALTERACAO]`: Percentual para alteração
- `[PERCENTUAL_DISSOLUCAO]`: Percentual para dissolução
- `[PLATAFORMA_COMUNICACAO]`: Plataforma de comunicação
- `[ASSINATURA_PARTICIPANTE]`: Assinatura digital do participante
- `[ASSINATURA_GESTOR]`: Assinatura digital do gestor
- `[ASSINATURA_ARBITRO]`: Assinatura digital do árbitro
- `[DATA_ASSINATURA_PARTICIPANTE]`: Data de assinatura do participante
- `[DATA_ASSINATURA_GESTOR]`: Data de assinatura do gestor
- `[DATA_ASSINATURA_ARBITRO]`: Data de assinatura do árbitro
- `[HASH_DOCUMENTO]`: Hash SHA256 do documento
- `[ENDERECO_MULTISIG]`: Endereço da multisig
- `[TIMESTAMP_CRIACAO]`: Timestamp de criação
- `[TIMESTAMP_ASSINATURA]`: Timestamp de assinatura
- `[TIMESTAMP_VIGENCIA]`: Timestamp de vigência
