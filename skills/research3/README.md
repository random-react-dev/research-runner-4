# Research service API

Plain JSON search and fetch endpoints; no MCP setup needed.

## Search

```sh
curl -G 'https://ask-gateway.r95426882.workers.dev/api/research/search?key=rk_rl-SOgOmj-QYMUYad54WAj0kx7Br9Lm1fVL6suD5P0k' \
  --data-urlencode 'q=Python pathlib official documentation'
```

## Fetch a page

```sh
curl -G 'https://ask-gateway.r95426882.workers.dev/api/research/fetch?key=rk_rl-SOgOmj-QYMUYad54WAj0kx7Br9Lm1fVL6suD5P0k' \
  --data-urlencode 'url=https://docs.python.org/3/library/pathlib.html'
```

Both return `{"status":"ok","results":[...],"guidance":"..."}`. The key also works as a Bearer token.
