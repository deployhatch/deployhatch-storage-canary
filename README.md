# Deploy Hatch Storage Canary

Disposable internal canary used to certify Deploy Hatch runtime disk-entitlement enforcement.

This application intentionally does almost nothing:
- no dependencies
- no build step
- starts with `npm start`
- listens on `PORT` (default 3000)
- `/` and `/health` return HTTP 200

The repository itself does **not** generate disk usage. Storage growth for the controlled B19C canary is performed externally against the exact disposable deployment workspace after all safety preconditions pass.

Do not use this repository for customer workloads.
