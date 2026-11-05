# Health eligibility rule evaluator

Run the tool locally from this folder:

```sh
node server.mjs
```

Open `http://127.0.0.1:4173` in a browser.

The tool reads the supplied source CSV, evaluates the selected multi-value rule, produces a fully expanded `.xlsx` file for review, and requires two explicit confirmations before rewriting the local compact-rule backend in `data/backend.json`.

The evaluator intentionally excludes `Version` and every later source column from the compact-rule logic. The exported comparison workbook preserves the original column layout.
