# Templates JSON - Protocolo PLS (PLIP-01)

## Template JSON Básico

### Contrato de Empréstimo Simples
```json
{
  "version": 1,
  "state": "Signed",
  "createdAt": 1640995200,
  "document": {
    "fileHash": "sha256_hash_do_documento_contrato",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ]
    }
  },
  "collateral": {
    "network": "bitcoin",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ]
    },
    "arbitratorsQuorum": 1,
    "multisigAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf"
  },
  "signatures": {
    "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f"
  }
}
```

## Template JSON com Comunicação (PLIP-02)

### Contrato de Empréstimo com Nostr
```json
{
  "version": 1,
  "state": "Signed",
  "createdAt": 1640995200,
  "document": {
    "fileHash": "sha256_hash_do_documento_contrato",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ]
    }
  },
  "collateral": {
    "network": "bitcoin",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ]
    },
    "arbitratorsQuorum": 1,
    "multisigAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf"
  },
  "communication": {
    "type": "nostr",
    "identifiers": {
      "clients": [
        "npub1a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "npub1b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "npub1c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ],
      "mediators": []
    }
  },
  "signatures": {
    "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f"
  }
}
```

## Template JSON para Contrato Híbrido

### Contrato com WoT + BJP + Seguro
```json
{
  "version": 1,
  "state": "Signed",
  "createdAt": 1640995200,
  "document": {
    "fileHash": "sha256_hash_do_documento_contrato_hibrido",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456",
        "03d4e5f678901234567890123456789012345678901234567890123456789012345678"
      ]
    }
  },
  "collateral": {
    "network": "bitcoin",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456",
        "03d4e5f678901234567890123456789012345678901234567890123456789012345678"
      ]
    },
    "arbitratorsQuorum": 2,
    "multisigAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf"
  },
  "communication": {
    "type": "nostr",
    "identifiers": {
      "clients": [
        "npub1a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "npub1b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "npub1c3d4e5f6789012345678901234567890123456789012345678901234567890123456",
        "npub1d4e5f678901234567890123456789012345678901234567890123456789012345678"
      ],
      "mediators": []
    }
  },
  "metadata": {
    "contractType": "loan_hybrid",
    "wot": {
      "enabled": true,
      "reputationThreshold": 50,
      "reputationReduction": 10
    },
    "insurance": {
      "enabled": true,
      "fundAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf",
      "coverageLimit": 0.05,
      "premiumRate": 1.0
    },
    "terms": {
      "loanAmount": 1000,
      "currency": "BRL",
      "collateralAmount": 0.01,
      "interestRate": 5.0,
      "termDays": 30
    }
  },
  "signatures": {
    "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "03d4e5f678901234567890123456789012345678901234567890123456789012345678": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f"
  }
}
```

## Estados do Contrato

### Estados Possíveis
```json
{
  "states": [
    "Created",
    "PartAccepted", 
    "Accepted",
    "PartSigned",
    "Signed",
    "PartFunded",
    "Funded",
    "Finished"
  ]
}
```

### Exemplo de Transição de Estados
```json
{
  "version": 1,
  "state": "PartFunded",
  "createdAt": 1640995200,
  "lastStateChange": 1640995800,
  "stateHistory": [
    {
      "state": "Created",
      "timestamp": 1640995200,
      "actor": "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890"
    },
    {
      "state": "Accepted",
      "timestamp": 1640995400,
      "actor": "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
    },
    {
      "state": "Signed",
      "timestamp": 1640995600,
      "actor": "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
    },
    {
      "state": "PartFunded",
      "timestamp": 1640995800,
      "actor": "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890"
    }
  ],
  "document": {
    "fileHash": "sha256_hash_do_documento_contrato",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ]
    }
  },
  "collateral": {
    "network": "bitcoin",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ]
    },
    "arbitratorsQuorum": 1,
    "multisigAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf"
  },
  "signatures": {
    "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f"
  }
}
```

## Template para Contrato de Seguro

### Contrato de Seguro Mútuo
```json
{
  "version": 1,
  "state": "Signed",
  "createdAt": 1640995200,
  "document": {
    "fileHash": "sha256_hash_do_documento_seguro",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456",
        "03d4e5f678901234567890123456789012345678901234567890123456789012345678",
        "02e5f67890123456789012345678901234567890123456789012345678901234567890"
      ]
    }
  },
  "collateral": {
    "network": "bitcoin",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456",
        "03d4e5f678901234567890123456789012345678901234567890123456789012345678",
        "02e5f67890123456789012345678901234567890123456789012345678901234567890"
      ]
    },
    "arbitratorsQuorum": 2,
    "multisigAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf"
  },
  "communication": {
    "type": "nostr",
    "identifiers": {
      "clients": [
        "npub1a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890"
      ],
      "arbitrators": [
        "npub1c3d4e5f6789012345678901234567890123456789012345678901234567890123456",
        "npub1d4e5f678901234567890123456789012345678901234567890123456789012345678",
        "npub1e5f67890123456789012345678901234567890123456789012345678901234567890"
      ],
      "mediators": []
    }
  },
  "metadata": {
    "contractType": "insurance_mutual",
    "insurance": {
      "fundAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf",
      "initialContribution": 0.005,
      "monthlyContribution": 0.001,
      "coverageLimit": 0.05,
      "premiumRate": 1.0
    },
    "terms": {
      "contractDuration": 365,
      "renewalTerms": "automatic",
      "cancellationNotice": 30
    }
  },
  "signatures": {
    "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "03d4e5f678901234567890123456789012345678901234567890123456789012345678": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "02e5f67890123456789012345678901234567890123456789012345678901234567890": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f"
  }
}
```

## Template para Contrato de Parceria P2P

### Contrato Exchange P2P
```json
{
  "version": 1,
  "state": "Signed",
  "createdAt": 1640995200,
  "document": {
    "fileHash": "sha256_hash_do_documento_parceria_p2p",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ]
    }
  },
  "collateral": {
    "network": "bitcoin",
    "pubkeys": {
      "clients": [
        "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ]
    },
    "arbitratorsQuorum": 1,
    "multisigAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf"
  },
  "communication": {
    "type": "nostr",
    "identifiers": {
      "clients": [
        "npub1a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890",
        "npub1b2c3d4e5f6789012345678901234567890123456789012345678901234567890123"
      ],
      "arbitrators": [
        "npub1c3d4e5f6789012345678901234567890123456789012345678901234567890123456"
      ],
      "mediators": []
    }
  },
  "metadata": {
    "contractType": "p2p_partnership",
    "wot": {
      "enabled": true,
      "reputationThreshold": 30,
      "reputationReduction": 5
    },
    "insurance": {
      "enabled": true,
      "fundAddress": "bc1p5d7rjsw7zt6rxymyav8zh46jrzgj8pg5wug9v2sxet4k9nyz3t9s6v0sqf",
      "coverageLimit": 0.02,
      "premiumRate": 0.5
    },
    "terms": {
      "partnershipDuration": 30,
      "maxTransactions": 10,
      "maxBitcoinAmount": 0.1,
      "maxFiatAmount": 5000,
      "currency": "BRL",
      "paymentMethod": "PIX"
    }
  },
  "signatures": {
    "02a1b2c3d4e5f6789012345678901234567890123456789012345678901234567890": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "03b2c3d4e5f6789012345678901234567890123456789012345678901234567890123": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f",
    "02c3d4e5f6789012345678901234567890123456789012345678901234567890123456": "304402203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f02203f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f3f"
  }
}
```

## Validação e Esquemas

### Esquema JSON Schema para Validação
```json
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "PLS Contract",
  "type": "object",
  "required": ["version", "state", "createdAt", "document", "collateral", "signatures"],
  "properties": {
    "version": {
      "type": "integer",
      "minimum": 1
    },
    "state": {
      "type": "string",
      "enum": ["Created", "PartAccepted", "Accepted", "PartSigned", "Signed", "PartFunded", "Funded", "Finished"]
    },
    "createdAt": {
      "type": "integer",
      "minimum": 0
    },
    "document": {
      "type": "object",
      "required": ["fileHash", "pubkeys"],
      "properties": {
        "fileHash": {
          "type": "string",
          "pattern": "^[a-f0-9]{64}$"
        },
        "pubkeys": {
          "type": "object",
          "required": ["clients", "arbitrators"],
          "properties": {
            "clients": {
              "type": "array",
              "items": {
                "type": "string",
                "pattern": "^[0-9a-f]{66}$"
              },
              "minItems": 2
            },
            "arbitrators": {
              "type": "array",
              "items": {
                "type": "string",
                "pattern": "^[0-9a-f]{66}$"
              },
              "minItems": 1
            }
          }
        }
      }
    },
    "collateral": {
      "type": "object",
      "required": ["network", "pubkeys", "arbitratorsQuorum", "multisigAddress"],
      "properties": {
        "network": {
          "type": "string",
          "enum": ["bitcoin", "liquid"]
        },
        "pubkeys": {
          "type": "object",
          "required": ["clients", "arbitrators"],
          "properties": {
            "clients": {
              "type": "array",
              "items": {
                "type": "string"
              }
            },
            "arbitrators": {
              "type": "array",
              "items": {
                "type": "string"
              }
            }
          }
        },
        "arbitratorsQuorum": {
          "type": "integer",
          "minimum": 0
        },
        "multisigAddress": {
          "type": "string"
        }
      }
    },
    "communication": {
      "type": "object",
      "properties": {
        "type": {
          "type": "string",
          "enum": ["nostr"]
        },
        "identifiers": {
          "type": "object",
          "properties": {
            "clients": {
              "type": "array",
              "items": {
                "type": "string"
              }
            },
            "arbitrators": {
              "type": "array",
              "items": {
                "type": "string"
              }
            },
            "mediators": {
              "type": "array",
              "items": {
                "type": "string"
              }
            }
          }
        }
      }
    },
    "signatures": {
      "type": "object",
      "patternProperties": {
        "^[0-9a-f]{66}$": {
          "type": "string"
        }
      }
    }
  }
}
```

## Notas de Implementação

### 1. Chaves Públicas
- **Formato**: Chaves secp256k1 em formato hexadecimal
- **Comprimento**: 66 caracteres (0x + 64 hex)
- **Validação**: Deve ser chave pública válida

### 2. Assinaturas
- **Formato**: Assinaturas DER em hexadecimal
- **Validação**: Deve ser assinatura válida do hash do contrato
- **Algoritmo**: ECDSA com curva secp256k1

### 3. Endereços Multisig
- **Formato**: Endereços Taproot (bech32m)
- **Validação**: Deve ser endereço válido para a rede especificada
- **Quorum**: Deve corresponder ao número de chaves necessárias

### 4. Timestamps
- **Formato**: Unix timestamp em segundos
- **Validação**: Deve ser timestamp válido
- **Ordem**: Estados devem seguir ordem cronológica

### 5. Hashes
- **Algoritmo**: SHA-256
- **Formato**: Hexadecimal em minúsculas
- **Validação**: Deve corresponder ao hash do documento
