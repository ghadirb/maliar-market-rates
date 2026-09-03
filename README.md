# Maliar market rates

This repository publishes a small, cached `rates.json` file for Maliar.
The Servix API key is stored only as a GitHub Actions secret named
`SERVIX_API_KEY`; never commit the key to this repository.

The scheduled workflow refreshes the file every two hours. GitHub Actions
schedule timing is approximate, so the timestamp in `rates.json` is the
source of truth.
