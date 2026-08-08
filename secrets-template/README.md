# Plannify secrets

## Usage

```bash
export ENVIRONMENT= FILE_NAME=
kubeseal --controller-name=sealed-secrets-controller --controller-namespace=kube-system --format yaml -f secrets/$ENVIRONMENT/$FILE_NAME.yaml -w yaml-applications/$ENVIRONMENT/secrets/$FILE_NAME.yaml
```
