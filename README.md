# Maliar market rates

This repository publishes a small, cached `rates.json` file for Maliar.

The Servix API key is stored only as a GitHub Actions secret named
`SERVIX_API_KEY`; never commit the key to this repository.

The Android app reads this public file automatically (no URL field for the user):

`https://raw.githubusercontent.com/ghadirb/maliar-market-rates/main/rates.json`

The scheduled workflow refreshes the file every two hours.
