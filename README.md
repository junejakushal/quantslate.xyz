# QuantSlate

**QuantSlate** is an educational algorithmic trading engine written in OCaml, inspired by the architectural patterns of Jane Street and Goldman Sachs SecDB. It uses the Zerodha Kite Connect API as a bridge to Indian capital markets for data ingestion and simulated (paper) trading.

> ⚠️ **Educational Project Disclaimer**  
> This is an educational and research implementation. It is **not** intended for production trading, nor does it constitute financial or investment advice. Trading in financial markets involves substantial risk of loss.

---

## Repository Structure

| Path | Description |
|------|-------------|
| `site/` | SvelteKit static website deployed to [quantslate.xyz](https://quantslate.xyz) |
| *(engine)* | *(OCaml trading engine source — coming soon)* |

---

## Website (`site/`)

The public site is built with **SvelteKit 5**, **Tailwind CSS v4**, and **TypeScript**. It is prerendered to static HTML via `@sveltejs/adapter-static`.

### Pages

- **Home** — Project introduction, inspirations, and tech stack
- **About** — Mission, why OCaml / SecDB / Kite, and educational intent
- **Architecture** — System design docs and OCaml module signatures
- **Disclaimer** — Full legal and educational disclaimers

### Deploying to Cloudflare Pages

1. Connect this repository to [Cloudflare Pages](https://pages.cloudflare.com/).
2. In the Pages dashboard, set the **Build configuration**:
   - **Build command:** `pnpm run build`
   - **Build output directory:** `build`
   - **Root directory:** `site`
3. Cloudflare Pages will detect `pnpm-lock.yaml` and use `pnpm` automatically.
4. Ensure the production environment variable `NODE_VERSION` matches `.nvmrc` (or leave it to auto-detect).

### Local Development

Use the **Debian (WSL)** shell where `fnm` and `pnpm` are installed:

```bash
cd site
pnpm install
pnpm run dev
```

Build for production:

```bash
pnpm run build
```

Static output is written to `site/build/`.

---

## Trading Engine (In Progress)

The engine is being designed as a modular, event-driven system in OCaml:

- **Market Data Adapter** — Zerodha Kite Connect WebSocket feeds
- **Normalized Order Book** — Immutable L1/L2/L3 book representation
- **SecDB-style Instrument Store** — Dependency graph of instruments, prices, and risk
- **Order Management System (OMS)** — Immutable event-sourced order lifecycle
- **Risk Gateway** — Pre-trade notional, position, and duplicate checks
- **Strategy Engine** — Pure functions over market state
- **Execution & Simulation** — Paper-trading fill simulation

---

## License

See [LICENSE](./LICENSE).
