# Contrato de Parceria P2P entre Exchange e Cliente por Período

Partes:

* Exchange P2P (Vendedor): \[NOME\_EXCHANGE], membro do \[NOME\_DA\_ORDEM]
* Cliente (Comprador): \[NOME\_CLIENTE], membro do \[NOME\_DA\_ORDEM]
* Árbitro: \[NOME\_ARBITRO], reconhecido pelo \[NOME\_DA\_ORDEM]

Data de Celebração: \[DATA\_INICIO]\
Período de Vigência: \[PERIODO\_DIAS] dias, até \[DATA\_FIM]

***

PREÂMBULOEste contrato estabelece os termos de uma parceria peer-to-peer (P2P) entre o Vendedor e o Comprador, ambos membros do \[NOME\_DA\_ORDEM], para a compra e venda de Bitcoin (BTC) com pagamento em Reais (BRL) via PIX, válida por um período de \[PERIODO\_DIAS] dias e limitada a \[LIMITE\_TRANSACOES] transações. O objetivo é proteger o Vendedor contra cancelamentos ou fraudes no pagamento, utilizando colaterais em BTC, reputação e arbitragem conforme os princípios da Private Law Society (PLS).

***

ARTIGO 1 - OBJETO DO CONTRATO1.1. O Vendedor concorda em vender até \[QUANTIDADE\_TOTAL\_BTC] BTC ao Comprador, em até \[LIMITE\_TRANSACOES] transações, por um valor total máximo de \[VALOR\_TOTAL\_FIAT] BRL, pago via PIX, durante o período de \[PERIODO\_DIAS] dias.\
1.2. O Comprador concorda em realizar os pagamentos e fornecer garantias conforme este contrato.

***

ARTIGO 2 - COLATERAL DO COMPRADOR2.1. O Comprador depositará \[COLATERAL\_BTC] BTC como colateral fixo em uma carteira multisig 2-de-3, no endereço \[ENDERECO\_MULTISIG], válido por todo o período de vigência.\
2.2. As chaves da carteira multisig serão mantidas por:

* a) Comprador: \[CHAVE\_COMPRADOR]
* b) Vendedor: \[CHAVE\_VENDEDOR]
* c) Árbitro: \[CHAVE\_ARBITRO]\
  2.3. O colateral será devolvido ao Comprador ao final do período (\[DATA\_FIM]), desde que todas as transações sejam concluídas sem incidentes, conforme Artigo 5.

***

ARTIGO 3 - CONDIÇÕES ESPECIAIS3.1. Seguro com Fundo: O Comprador pode optar pelo fundo de seguro do \[NOME\_DA\_ORDEM], reduzindo o colateral em \[PERCENTUAL\_SEGURO]%, mediante pagamento de uma taxa única de \[TAXA\_SEGURO]% sobre \[QUANTIDADE\_TOTAL\_BTC], depositada em \[ENDERECO\_FUNDO] no início do contrato.\
3.2. Reputação: Membros com alta reputação no \[NOME\_DA\_ORDEM] terão o colateral reduzido em \[PERCENTUAL\_REPUTACAO]%, conforme avaliação em \[PLATAFORMA\_REPUTACAO].\
3.3. Associação: Por serem membros do \[NOME\_DA\_ORDEM], o colateral será ajustado em \[PERCENTUAL\_ASSOCIACAO]%.

***

ARTIGO 4 - EXECUÇÃO DAS TRANSAÇÕES4.1. Para cada transação dentro do limite de \[LIMITE\_TRANSACOES]:

* a) O Comprador notificará o Vendedor via \[PLATAFORMA\_ASSINATURA] com o valor em BTC desejado (\[QUANTIDADE\_BTC\_TRANSACAO]) e o correspondente em BRL (\[VALOR\_FIAT\_TRANSACAO]).
* b) O Comprador realizará o PIX de \[VALOR\_FIAT\_TRANSACAO] BRL para \[CONTA\_PIX\_VENDEDOR] em até \[PRAZO\_HORAS] horas após a solicitação.
* c) O Vendedor confirmará o PIX e enviará \[QUANTIDADE\_BTC\_TRANSACAO] BTC para \[ENDERECO\_COMPRADOR] em até \[PRAZO\_CONFIRMACAO] horas.\
  4.2. O total de BTC vendido não excederá \[QUANTIDADE\_TOTAL\_BTC], e o número de transações não ultrapassará \[LIMITE\_TRANSACOES].

***

ARTIGO 5 - PROTEÇÃO CONTRA CANCELAMENTO OU FRAUDE5.1. O Vendedor deve fornecer prova de recebimento de cada PIX (ex.: comprovante bancário) via \[PLATAFORMA\_ASSINATURA] antes de liberar o BTC.\
5.2. Se o Comprador cancelar um PIX após o envio do BTC em qualquer transação:

* a) O Vendedor terá direito a \[PERCENTUAL\_PENALIDADE]% do colateral (\[COLATERAL\_BTC]) por transação fraudulenta, até o limite do valor perdido.
* b) O Comprador deve notificar problemas com o PIX em até \[PRAZO\_NOTIFICACAO] horas, ou a penalidade será aplicada.\
  5.3. O colateral remanescente será devolvido ao Comprador em \[DATA\_FIM], após ajustes por eventuais penalidades.

***

ARTIGO 6 - INADIMPLÊNCIA6.1. Se o Comprador não realizar o PIX de uma transação solicitada dentro de \[PRAZO\_HORAS] horas, o Vendedor poderá reter \[PERCENTUAL\_PENALIDADE]% do colateral como multa, limitada ao valor da transação não cumprida.\
6.2. Se o Vendedor não liberar o BTC após confirmação do PIX em \[PRAZO\_CONFIRMACAO] horas, o colateral será devolvido integralmente ao Comprador, e o Vendedor será penalizado via reputação no \[NOME\_DA\_ORDEM].

***

ARTIGO 7 - ENCERRAMENTO DO CONTRATO7.1. O contrato termina em \[DATA\_FIM] ou ao atingir \[LIMITE\_TRANSACOES], o que ocorrer primeiro.\
7.2. O colateral (\[COLATERAL\_BTC] BTC) será liberado ao Comprador em até \[PRAZO\_LIBERACAO] horas após o término, salvo ajustes por inadimplência ou fraude.

***

ARTIGO 8 - RISCO DE FLUTUAÇÃO DE PREÇO8.1. Ambas as partes aceitam que a flutuação de preço do BTC ou BRL é um risco mútuo e não será objeto de disputa ou arbitragem.

***

ARTIGO 9 - ARBITRAGEM9.1. Disputas (ex.: cancelamento fraudulento, atrasos) serão resolvidas pelo árbitro \[NOME\_ARBITRO], com base em evidências via \[PLATAFORMA\_ASSINATURA].\
9.2. A decisão do árbitro é final, exceto em questões de flutuação de preço (Artigo 8).\
9.3. O prazo para resolução é de \[PRAZO\_ARBITRAGEM] dias após notificação.

***

ARTIGO 10 - ASSINATURAS10.1. Este contrato é assinado digitalmente via \[PLATAFORMA\_ASSINATURA].

* Vendedor (Exchange): \[ASSINATURA\_EXCHANGE]
* Comprador (Cliente): \[ASSINATURA\_CLIENTE]
* Árbitro: \[ASSINATURA\_ARBITRO]

***

ARTIGO 11 - DISPOSIÇÕES GERAIS11.1. O colateral ajustado será \[COLATERAL\_AJUSTADO] BTC, após aplicar seguro, reputação e associação.\
11.2. O fundo de seguro é gerido pelo \[NOME\_DA\_ORDEM] em \[ENDERECO\_FUNDO].\
11.3. Todas as comunicações devem ser registradas em \[PLATAFORMA\_ASSINATURA].
