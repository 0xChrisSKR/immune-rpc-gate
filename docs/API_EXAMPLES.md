# API Examples

This repository documents a gateway design. Public examples are interface contracts and reviewer-facing artifact requests, not a claim that a public production gateway is deployed.

## Public Artifact Requests

README request:

```bash
curl -L "https://raw.githubusercontent.com/0xChrisSKR/immune-rpc-gate/master/README.md"
```

Architecture document request:

```bash
curl -L "https://raw.githubusercontent.com/0xChrisSKR/immune-rpc-gate/master/docs/ARCHITECTURE.md"
```

Career mapping request:

```bash
curl -L "https://raw.githubusercontent.com/0xChrisSKR/immune-rpc-gate/master/docs/CAREER_MAPPING.md"
```

Representative response shape:

```json
{
  "repository": "immune-rpc-gate",
  "artifact": "public engineering showcase",
  "source": "https://github.com/0xChrisSKR/immune-rpc-gate",
  "claimBoundary": "verifiable public material only"
}
```


## Design Contract Example

Request:

```bash
curl -X POST "https://example.invalid/rpc-gate/read" \
  -H "Content-Type: application/json" \
  -d '{"method":"getHealth","mode":"read-only"}'
```

Response shape:

```json
{
  "mode": "DEGRADED",
  "readOnly": true,
  "upstreamHealthy": false,
  "action": "serve-safe-read-or-return-503"
}
```

This is a design contract example, not a deployed public endpoint.
