# Steps to reproduce

```bash
kubectl apply -f stepaction.yaml
kubectl apply -f test.yaml
```
To check output log

```bash
tkn tr logs
```

Expected behavior:
Fail the run because the commands param expects a list but a string is passed instead

Actual Behavior:
Run succeeds and the logs show the default value instead