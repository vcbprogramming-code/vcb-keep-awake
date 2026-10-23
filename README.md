# vcb-keep-awake

Keeps the VCB Connect **UAT** server on Render's free plan awake by visiting its health address
(`/api/health`, no data, no sign-in) every 5 minutes. See `.github/workflows/keep-uat-awake.yml`.

- UAT only. The production server shares the same ~750 free Render hours a month; keeping both awake would use them
  up and stop both. Production should be on a paid plan before launch.
- To stop it: Actions → "Keep UAT awake" → ⋯ → Disable workflow (or delete this repository).
