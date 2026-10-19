# 

# \# Cloud Run Mapping

# 

# \## Configuration Variables

# 

# \- `LOG\_LEVEL`: Non-secret application logging configuration.

# \- `PORT`: Application port; defaults to `3000` if not provided by the runtime.

# 

# \## Secrets

# 

# \- `DATABASE\_URL`: Database connection string. Store in Google Secret Manager if it contains credentials.

# \- `API\_KEY`: API credential. Store in Google Secret Manager.

# 

# \## Deployment Notes

# 

# \- Supply non-secret values through Cloud Run environment variables.

# \- Supply sensitive values through Secret Manager-backed environment variables.

# \- Never commit `.env` or embed secret values in the Dockerfile.

# \- `.env.example` must contain placeholders only.

# 

