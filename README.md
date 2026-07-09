# VibeNest Template: ntfy

This is a thin VibeNest-ready deploy adapter for [ntfy](https://github.com/binwiederhier/ntfy).

It does not fork or modify ntfy. The repo only provides deploy-safe Docker defaults for a personal notification server:

- official image: `binwiederhier/ntfy:latest`
- app port: `80`
- persistent cache/auth database volume
- deny-by-default auth baseline

## VibeNest notes

One-click deploy stays disabled until smoke confirms the public URL opens ntfy and the first-user/auth flow is safe. After deploy, create users with the ntfy CLI or a controlled platform recipe before exposing private topics.

## Upstream

- Product: https://github.com/binwiederhier/ntfy
- Docs: https://docs.ntfy.sh/install/
- Config docs: https://ntfy.sh/docs/config/
