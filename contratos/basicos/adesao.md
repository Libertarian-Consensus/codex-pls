# Contrato de Adesão

**Versão:** 1.0  
**Data:** [DATA_CONTRATO]  
**Protocolo:** PLS (PLIP-01)

## Partes

- **Candidato:** [NOME_CANDIDATO], chave pública: [CHAVE_CANDIDATO]
- **Membro Convidante:** [NOME_CONVIDANTE], chave pública: [CHAVE_CONVIDANTE]
- **Árbitro:** [NOME_ARBITRO], chave pública: [CHAVE_ARBITRO]

## Objetivo

Este contrato estabelece os termos de adesão ao [NOME_ASSOCIACAO], uma associação privada que opera sob os princípios da [Private Law Society (PLS)](http://privatelawsociety.net).

## Termos de Adesão

### 1. Requisitos
- **Convite Formal**: Convite assinado por membro ativo
- **Chave Pública**: Chave pública registrada no protocolo
- **Colateral Inicial**: [COLATERAL_INICIAL] BTC depositado
- **Aprovação**: Aprovação do conselho da associação

### 2. Processo de Adesão
1. Candidato recebe convite formal
2. Candidato deposita colateral inicial
3. Conselho avalia candidatura
4. Aprovação em até 7 dias
5. Contrato assinado por todas as partes

### 3. Colateral de Adesão
- **Valor**: [COLATERAL_INICIAL] BTC
- **Multisig**: 2-de-3 (candidato + membro + árbitro)
- **Endereço**: [ENDERECO_MULTISIG]
- **Finalidade**: Garantia de boa conduta

## Direitos e Deveres

### 1. Direitos do Membro
- Utilizar reputação da associação
- Acessar fundo de seguro (se aplicável)
- Solicitar arbitragem em disputas
- Participar de decisões da associação
- Recuperar colateral ao sair

### 2. Deveres do Membro
- Manter conduta honesta
- Respeitar decisões arbitrais
- Reportar transações no sistema
- Cumprir obrigações contratuais
- Preservar reputação coletiva

## Cláusulas Modulares

### Cláusula de Colateral
*[Incluir cláusula de colateral básica - ver [clausulas/colateral.md](../../clausulas/colateral.md)]*

**Colateral:** [COLATERAL_INICIAL] BTC depositado em multisig 2-de-3

### Cláusula de Arbitragem
*[Incluir cláusula de arbitragem básica - ver [clausulas/arbitragem.md](../../clausulas/arbitragem.md)]*

**Árbitro:** [NOME_ARBITRO] para disputas relacionadas à adesão

### Cláusula de Comunicação
*[Incluir cláusula de comunicação básica - ver [clausulas/comunicacao.md](../../clausulas/comunicacao.md)]*

**Plataforma:** [PLATAFORMA_COMUNICACAO] para comunicações oficiais

## Sistema de Reputação

### 1. Avaliação Inicial
- **Base**: Histórico de transações
- **Recomendações**: Avaliações de membros existentes
- **Critérios**: Honestidade, confiabilidade, experiência

### 2. Manutenção de Reputação
- **Transações Bem-sucedidas**: +5 pontos
- **Violações**: -10 pontos
- **Recomendações**: +3 pontos
- **Disputas Perdidas**: -5 pontos

### 3. Benefícios por Reputação
- **Alta Reputação (>50)**: Redução de colateral em 10%
- **Reputação Premium (>100)**: Benefícios adicionais
- **Baixa Reputação (<20)**: Restrições ou expulsão

## Expulsão e Saída

### 1. Expulsão
- **Descumprimento Grave**: Violação de termos contratuais
- **Reputação Negativa**: Reputação abaixo de 0 pontos
- **Decisão Arbitral**: Decisão de árbitro independente
- **Confisco de Colateral**: Colateral pode ser confiscado

### 2. Saída Voluntária
- **Notificação**: 30 dias de antecedência
- **Quitação**: Resolução de pendências
- **Liberação**: Colateral liberado após quitação
- **Reputação**: Reputação mantida se positiva

## Alterações ao Contrato

### 1. Processo de Alteração
- **Proposta**: Qualquer membro pode propor alterações
- **Votação**: 75% de aprovação necessária
- **Peso**: Votos ponderados por reputação/colateral
- **Implementação**: Alterações em vigor após aprovação

### 2. Notificação
- **Prazo**: 30 dias de antecedência
- **Método**: [PLATAFORMA_COMUNICACAO]
- **Aceitação**: Assinatura digital necessária

## Assinaturas Digitais

### Candidato
- **Chave pública:** [CHAVE_CANDIDATO]
- **Assinatura:** [ASSINATURA_CANDIDATO]
- **Data:** [DATA_ASSINATURA_CANDIDATO]

### Membro Convidante
- **Chave pública:** [CHAVE_CONVIDANTE]
- **Assinatura:** [ASSINATURA_CONVIDANTE]
- **Data:** [DATA_ASSINATURA_CONVIDANTE]

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
- **Chaves:** [CHAVE_CANDIDATO], [CHAVE_CONVIDANTE], [CHAVE_ARBITRO]

### Timestamps
- **Criado:** [TIMESTAMP_CRIACAO]
- **Assinado:** [TIMESTAMP_ASSINATURA]
- **Vigência:** [TIMESTAMP_VIGENCIA]

## Variáveis de Template

- `[DATA_CONTRATO]`: Data de criação do contrato
- `[NOME_CANDIDATO]`: Nome ou pseudônimo do candidato
- `[NOME_CONVIDANTE]`: Nome ou pseudônimo do convidante
- `[NOME_ARBITRO]`: Nome ou pseudônimo do árbitro
- `[CHAVE_CANDIDATO]`: Chave pública do candidato
- `[CHAVE_CONVIDANTE]`: Chave pública do convidante
- `[CHAVE_ARBITRO]`: Chave pública do árbitro
- `[NOME_ASSOCIACAO]`: Nome da associação
- `[COLATERAL_INICIAL]`: Colateral inicial em BTC
- `[ENDERECO_MULTISIG]`: Endereço da multisig
- `[PLATAFORMA_COMUNICACAO]`: Plataforma de comunicação
- `[ASSINATURA_CANDIDATO]`: Assinatura digital do candidato
- `[ASSINATURA_CONVIDANTE]`: Assinatura digital do convidante
- `[ASSINATURA_ARBITRO]`: Assinatura digital do árbitro
- `[DATA_ASSINATURA_CANDIDATO]`: Data de assinatura do candidato
- `[DATA_ASSINATURA_CONVIDANTE]`: Data de assinatura do convidante
- `[DATA_ASSINATURA_ARBITRO]`: Data de assinatura do árbitro
- `[HASH_DOCUMENTO]`: Hash SHA256 do documento
- `[TIMESTAMP_CRIACAO]`: Timestamp de criação
- `[TIMESTAMP_ASSINATURA]`: Timestamp de assinatura
- `[TIMESTAMP_VIGENCIA]`: Timestamp de vigência
