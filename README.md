# Tari Community Discourse

A self-hosted [Discourse](https://www.discourse.org/) forum for the Tari community, deployed at `community.tari.com`.

## What this repo is

This repo tracks the setup, deployment configuration, and documentation for the Tari community forum. It is not the Discourse codebase itself — it contains the deployment playbook (docker-compose, nginx config, or equivalent), seeding scripts, configuration files, and operational documentation needed to stand up and hand over a production instance.

## Acceptance criteria

A submission must demonstrably satisfy all six criteria to be accepted:

1. **SSL live** — HTTPS on `community.tari.com` with a valid cert (Let's Encrypt or equivalent), no HTTP fallback.
2. **Categories seeded** — Forum categories matching the Tari community structure are present at first boot.
3. **Trust levels configured** — Discourse trust level thresholds are tuned for a new community (not Discourse defaults).
4. **GitHub SSO** — Users can sign in via GitHub OAuth; email/password login policy is documented.
5. **Backup and restore tested** — A backup has been created, restored to a clean instance, and the procedure is documented step-by-step in this repo.
6. **Tari branding applied** — Logo, colour scheme, and site title match Tari brand guidelines.

## Infrastructure

- **VPS**: Provided by Tari Labs (credentials shared privately after PR is opened)
- **Domain**: `community.tari.com`
- **Admin handover**: Credentials delivered to @metalaureate at completion

## Contributing

Open a PR against `main`. The submission that best meets all six acceptance criteria will be selected. See acceptance criteria above.