# architecture // the machine without the keys

ONE4ALL uses a lean event graph. Public facts enter through allowlisted readers. Deterministic code checks identity, freshness, duplication, policy, and limits before any model sees an event.

```text
Solana / RevShare / X / site event
                 │
                 ▼
              Watcher
      parse · dedupe · timestamp
                 │
                 ▼
           deterministic policy
          ╱          │          ╲
     ignore        stage       escalate
                    │
             ┌──────┴──────┐
             ▼             ▼
        OMNI CLAW      OMNI VAULT
         culture       operations
             └──────┬──────┘
                    ▼
            OMNI THIRD EYE
        facts · limits · duplicate check
                    │
                    ▼
       draft / approved bounded action
                    │
                    ▼
              durable audit
```

## public signal contract

This is a **schema example**, not a live event or transaction receipt:

```json
{
  "schema": "one4all.signal.v1",
  "id": "example_public_signal",
  "observedAt": "2026-01-01T00:00:00.000Z",
  "source": {
    "kind": "public-chain-reader",
    "network": "solana-mainnet"
  },
  "event": {
    "name": "reward.distribution.confirmed",
    "status": "verified"
  },
  "evidence": {
    "publicUrl": "https://explorer.solana.com/",
    "confirmation": "finalized"
  }
}
```

Collectors, private endpoints, prompts, deployment controls, policy internals, financial execution logic, databases, and credentials are deliberately excluded from this repository.

## why it stays lean

- Core reads and policy still work when model providers are offline.
- Models are used for language and bounded judgment, not accounting or permission.
- Retries preserve the same idempotency key.
- Public outputs keep evidence, timestamps, and receipts.
- High-risk actions stop at an owner gate.

The result is autonomy with a seatbelt: the cats can watch and speak without becoming a wallet.
