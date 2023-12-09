# Indexing
- Mappings
    - ``bbuy_products.json``: 28.18 mins
    - ``bbuy_products_no_map.json``: 21.52 mins
- Refresh Interval with ``bbuy_products_no_map.json`
    - ``-1``: 17.08 mins
    - ``1s``: 18.28 mins
    - ``60s``: 16.22
- Batch size with ``bbuy_products_no_map.json`` and refresh interval ``-1``
    - ``400``: 16.81 mins
- Workers with ``bbuy_products_no_map.json`` and refresh interval ``-1``
    - ``32``: It took ages :)

# Querying
- 10000 queries - baseline: 1.9973403266999716 mins
- No fuzzy name: 1.678468009266726 mins
- No func score: 1.1903781125334112 mins
- Multi-match - name and short desc: 0.9920639620500878 mins