# Solution

- Increase `storage` in `persistentvolumeclaim.yaml` to 1Gi.
- Add a selector to the `service.yaml`:

```
  selector:
    app: web-app
```