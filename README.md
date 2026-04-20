# Transformd

Customer-facing artifacts and issue tracker for **Transformd** — the AI-powered observability pipeline.

> **Note**: This repository exists for:
> - 🐛 [Issue tracking](https://github.com/transformd-co/transformd/issues)
> - 📦 [Release artifacts](https://github.com/transformd-co/transformd/releases) (binaries, `.deb`, `.rpm`, SBOMs)
> - 🐳 [Container images](https://github.com/orgs/transformd-co/packages) (`ghcr.io/transformd-co/transformd`)

## Install the agent

### Linux (native package — recommended)

```bash
curl -sSL https://beta.transformd.co/install.sh | sudo TRANSFORMD_API_KEY=<your-key> bash
```

### Container

```bash
docker pull ghcr.io/transformd-co/transformd:latest
```

### Verify signatures (Sigstore cosign)

```bash
cosign verify ghcr.io/transformd-co/transformd:vX.Y.Z \
  --certificate-oidc-issuer https://gitlab.com \
  --certificate-identity-regexp '.*nextr-consulting/transformd.*'
```

## Documentation

Full docs: https://beta.transformd.co/docs

## Support

- Bug reports + feature requests: [Issues](https://github.com/transformd-co/transformd/issues)
- Security disclosures: security@transformd.co
