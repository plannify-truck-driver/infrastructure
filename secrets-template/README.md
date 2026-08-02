# Plannify secrets

## Usage

```bash
kubeseal --controller-name=sealed-secrets-controller --controller-namespace=kube-system --format yaml -f secrets-template/<environment>/<secret-file-name>.yaml -w yaml-applications/<environment>/secrets/<secret-file-name>.yaml
```
