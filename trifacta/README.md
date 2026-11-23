# TRIFACTA

**The live API.** The KATIE record with ERIE on top.

TRIFACTA is the API that serves VOLSHI's trust layer. Ask a question and it answers from the record, and every answer carries its proof: the KID, the birth stamp, the trust score, and the source it came from. If the record does not know, it says so. It never guesses.

## Live

**https://trifacta-api.onrender.com**

- `GET /health` — open, no key needed
- `POST /ask` — ask a question, get an answer with provenance
- `POST /chat` — talk to a persona (Brunel and Caveman are live)
- `POST /accounts` — create an account with fields
- `POST /update` — write a field, authority-graded
- `GET /record/{account_id}` — full history with KID and entry hash
- `GET /lessons`, `GET /accounts`, `GET /insights`, `/search` — read the record

Every route except `/health` and `/config` needs an `X-API-Key` header.

## The name

TRIFACTA is tri plus fact. With ERIE it is nothing but facts, so it is the trifecta.

## Demo data

The live service carries a 5-person demo cast: five people with arcs the record has lived through. The bulk pool is not loaded.

## Systems

TRIFACTA is built from [KATIE](../katie/) (the record), [ERIE](../erie/) (retrieval and investigation), [ELLE](https://github.com/CenturionOversight/ELLE) (learning), and [ARCHE](../arche/) (the engine).

---

Copyright © 2026 VOLSHI. All rights reserved.
