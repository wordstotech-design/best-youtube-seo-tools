# Contributing

This is a living, vendor-neutral list of YouTube SEO tools. Corrections and additions are welcome.

## How to add or fix a tool

1. Edit [tools.yaml](tools.yaml). Each entry has these fields:
   - `name`, `url` (optional), `type`, `free`, `price_from`, `best_for`
2. Regenerate the comparison table:
   ```bash
   python render_table.py --write
   ```
   This rewrites only the block between the `<!-- TABLE:START -->` and `<!-- TABLE:END -->` markers in `README.md`.
3. Open a pull request describing the change and the source for any pricing or feature claim.

## Ground rules

- **Factual and current.** Pricing and features change often. Cite the vendor page you took a number from.
- **Vendor-neutral tone.** Describe what a tool is best for, not who it beats. No superlatives without a fact behind them.
- **No affiliate links.** Tool URLs point to the vendor's own site only.
- **One entry per tool.** Update the existing entry rather than adding a duplicate.

## Local setup

```bash
pip install pyyaml
python render_table.py        # preview the table
python render_table.py --write  # write it into README.md
```
