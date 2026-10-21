# Service retired — 2026-10-21

The `brother-scanner` service is no longer needed and was stopped by owner request.
Its container restart policy is disabled. Compose excludes it from normal
startup through the `retired` profile. Containers and data are retained.

Do not restart it without first patching its PHP runtime. A deliberate restart
would require `docker compose --profile retired up -d --no-deps brother-scanner`.
