# Setup the garage server

1. Get the garage status

```bash
kubectl exec -n plannify-2 garage-0 -- /garage status
```

2. Assign a node capacity

```bash
kubectl exec -n plannify-2 garage-0 -- /garage layout assign -z dc1 -c 5G <node_id>
```

3. Show the layout

```bash
kubectl exec -n plannify-2 garage-0 -- /garage layout show
```

4. Apply the layout

```bash
kubectl exec -n plannify-2 garage-0 -- /garage layout apply --version 1
```

5. Create a token for the garage-ui

```bash
kubectl exec -n plannify-2 garage-0 -- /garage admin-token create garage-ui
```
