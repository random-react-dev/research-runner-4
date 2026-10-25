# Research service API

Plain JSON search and fetch endpoints; no key or setup needed.

## Search

```sh
curl -G 'https://ask-gateway.r95426882.workers.dev/api/research/search' \
  --data-urlencode 'q=Python pathlib official documentation'
```

## Fetch a page

```sh
curl -G 'https://ask-gateway.r95426882.workers.dev/api/research/fetch' \
  --data-urlencode 'url=https://docs.python.org/3/library/pathlib.html'
```

Both return `{"status":"ok","results":[...],"guidance":"..."}`.
