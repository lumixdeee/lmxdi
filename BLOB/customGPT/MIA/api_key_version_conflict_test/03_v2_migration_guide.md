# Acme SDK v2 Migration Guide

**Version:** 2.0  
**Published:** 2025-02-10  
**Status:** Current official documentation

## API key configuration

In v2, store the API key in the `ACME_API_KEY` environment variable.

Example:

```bash
export ACME_API_KEY="YOUR_API_KEY"
```

The `config.yaml` API-key field is deprecated in v2. It remains documented only as v1 historical behavior and should not be recommended for new v2 setups.

## What changed

- v1: API key stored in `config.yaml`
- v2: API key moved to `ACME_API_KEY`
- v2 status of `config.yaml`: deprecated
