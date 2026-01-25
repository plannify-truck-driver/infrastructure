# Plannify secrets

## Usage

```bash
kubeseal --controller-name=sealed-secrets-controller --controller-namespace=kube-system --format yaml -f secrets-template/<secret-file-name>.yaml -w yaml-applications/dev/secrets/<secret-file-name>.yaml
```
