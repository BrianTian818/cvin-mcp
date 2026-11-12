# CVIN — MCP Server

**GPU compute-asset identity registry**: resolve device identity, verify history, buy official reports.

- **MCP endpoint**: `https://cvin.org/mcp` (streamable-http)
- **Website**: https://cvin.org
- **Official MCP Registry**: `io.github.BrianTian818/cvin` (status: active)
- **Protocol**: MCP over Streamable HTTP + [x402](https://www.x402.org) micropayments (USDC, machine-payable)

## What is CVIN?

CVIN gives every piece of compute hardware — a single GPU card, a full server, or an entire rack —
a **cross-operator, machine-verifiable identity** and a **history anyone can independently recompute**.
Think "VIN for GPUs": before you rent or buy capacity on the secondary market, check the device's
identity and history first.

## Tools

| Tool | Price | Description |
| --- | --- | --- |
| `cvin_resolve` / `cvin_resolve_batch` | Free (batch up to 200) | Resolve device identity, get combined snapshot |
| `cvin_history` | $0.05/req (x402) | Full history timeline of a device |
| `cvin_verify` | $0.05/req (x402) | Verify claimed identity against registry |
| `cvin_report` | $2/report (x402) | Official verification report |
| `cvin_buy_key` | $10 / 30 days (x402) | Self-serve subscription key |
| `cvin_encode` / `cvin_identity` / `cvin_permits` | Free | Encoding standards, identity scheme, permits |

## Connect

Point any MCP-compatible client at:

```
https://cvin.org/mcp
```

## Server metadata

See [`server.json`](./server.json) — the listing already published to the official
[MCP Registry](https://registry.modelcontextprotocol.io) and mirrored by Glama,
MCP Marketplace, and other directories.
