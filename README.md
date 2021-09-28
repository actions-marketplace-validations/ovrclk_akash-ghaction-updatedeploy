# Update Akash Deploy

Sets up the Akash CLI for Github Action use. Installs the latest Akash CLI, Imports Keys, and deployment Certificates.

## Inputs

### `GITHUB_TOKEN`

**Required** The github runner token

### `AKASH_WALLET_KEY`

**Required** The pem text of the akash wallet key

### `AKASH_WALLET_KEY_PASSWORD`

**Required** The password encrypting the wallet key pem

### `AKASH_DEPLOY_CERTIFICATE`

**Required** The deploy certificate pem text

## Example usage

```yaml
- name: Akash on Github Actions Setup
  uses: ovrclk/akash-ghaction-setup
  with:
    GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
    AKASH_WALLET_KEY: ${{secrets.AKASH_WALLET_KEY}}
    AKASH_WALLET_KEY_PASSWORD: ${{secrets.AKASH_WALLET_KEY_PASSWORD}}
    AKASH_DEPLOY_CERTIFICATE: ${{secrets.AKASH_DEPLOY_CERTIFICATE}}
```
