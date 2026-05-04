# Publishing Setup

This folder is ready to publish through any existing free static host or compliant free public channel.

Local files:

- `public/ai-growth-ops/index.html`
- `public/ai-growth-ops/acquisition_content.md`
- `public/ai-growth-ops/acquisition_content_packet.json`

Activation rule:

Do not treat these files as production traction until the offer page is reachable at a real public URL or posted through a configured free public channel. After publishing, set `AGENTIC_SYSTEMS_PUBLIC_OFFER_URL` or `AGENTIC_SYSTEMS_PUBLIC_SITE_URL` outside the repo and rerun:

```bash
python3 -m agentic_systems.cli production-status --run latest
python3 -m agentic_systems.cli production-next-action --run latest
```

## Zero-Budget Channel Worksheet

Fill this out outside the repo before counting the channel as live:

- Selected free channel or public URL:
- Why it costs `$0` and is controlled by the operator:
- Public location where the offer is visible:
- Where inbound opt-in replies will be copied for validation:

Allowed non-secret references:

- `AGENTIC_SYSTEMS_PUBLIC_OFFER_URL=https://...`
- `AGENTIC_SYSTEMS_PUBLIC_SITE_URL=https://...` plus `AGENTIC_SYSTEMS_PUBLIC_SITE_DIR=/absolute/path`
- `AGENTIC_SYSTEMS_CONNECTED_FREE_CHANNELS=existing-public-profile-or-community`

Do not include passwords, API tokens, session cookies, private keys, paid ad settings, fake proof, payment authorization, or channels where commercial posts are prohibited.

Post-publication verification:

```bash
python3 -m agentic_systems.cli production-status --run latest
python3 -m agentic_systems.cli production-next-action --run latest
python3 -m agentic_systems.cli next-source-task --run latest
```
