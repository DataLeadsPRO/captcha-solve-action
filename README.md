# DataLeads Captcha Solver (GitHub Action)

Solve a captcha challenge on a URL via the DataLeads CaptchaFlow engine and return the token as JSON.

Calls the DataLeads API endpoint `POST /v1/captcha/solve` and writes the JSON response to `dataleads-result.json` plus the `result` output.

## Usage

```yaml
steps:
  - uses: DataLeadsPRO/captcha-solve-action@v1
    with:
      url: https://example.com
      api_key: ${{ secrets.DATALEADS_API_KEY }}
```

Get a client key at [data.dataleads.pro](https://data.dataleads.pro).

## License

MIT
