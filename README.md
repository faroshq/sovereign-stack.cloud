# sovereign-stack.cloud

Landing page for the [Sovereign Stack](https://github.com/faroshq/neocloud) — an open source reference architecture for building sovereign cloud platforms.

## What is Sovereign Stack?

A 100% open-source, CNCF-native reference architecture for turning commodity hardware into a multi-tenant cloud platform. Three composable layers:

- **Infrastructure** — Bare metal to Kubernetes (Metal3, Cilium, Rook-Ceph, KubeVirt)
- **Platform** — Multi-tenant cloud APIs via kcp (Compute, VM, Notebook, GPU, Storage)
- **Production** — Billing, monitoring, identity (OpenMeter, Zitadel, Prometheus)

No proprietary components. No vendor lock-in. Designed for EU digital sovereignty.

See the [full architecture docs](https://github.com/faroshq/neocloud).

## Development

Prerequisites: Node.js 22+

```bash
npm install
npm run dev        # http://localhost:4321
```

## Build

```bash
npm run build      # Output in ./dist
```

## Deployment

Deployed to [Cloudflare Pages](https://pages.cloudflare.com/) on push to `main`.

Set these secrets in GitHub Actions:
- `CLOUDFLARE_API_TOKEN`
- `CLOUDFLARE_ACCOUNT_ID`

## Tech Stack

- [Astro](https://astro.build) — static site generator
- [Tailwind CSS](https://tailwindcss.com) — utility-first CSS
- [Cloudflare Pages](https://pages.cloudflare.com/) — edge deployment

## License

Apache 2.0
