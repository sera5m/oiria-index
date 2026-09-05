# oiria-index

AUR-shaped catalog for Vulcan / OIRIA watch scripts.
You (sera5m) **read the PR and merge**. Nothing is auto-approved.

Desktop companions only serve packages that exist under `approved/`.

## Folders

| path | meaning |
|------|--------|
| `pending/<id>/` | submitted, not shipped |
| `approved/<id>/` | you merged it; companions may serve |
| `rejected/<id>/` | looked at, no |

Each package folder:

```
<id>/
  pkg.json     # id, version, kind, note
  main.vul     # or other payload
```

## Submit

1. Fork (or branch).
2. Add `pending/your_id/pkg.json` + `main.vul`.
3. Open a PR against `main`.
4. Maintainer moves the folder to `approved/` or `rejected/` and merges.

Do not put binaries. Source only. No `fs.delete` / power scripts.
