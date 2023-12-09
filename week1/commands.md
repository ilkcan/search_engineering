- ``export HOST=localhost``
- ``export BBUY_DATA=/workspace/datasets/product_data/products``

- ``curl -k -X DELETE -u admin:admin https://${HOST}:9200/bbuy_products``

- ``curl -k -X PUT -u admin:admin -H 'Content-Type: application/json' -d @week1/bbuy_products.json "https://${HOST}:9200/bbuy_products"``
- ``curl -k -X PUT -u admin:admin -H 'Content-Type: application/json' -d @week1/bbuy_products_no_map.json "https://${HOST}:9200/bbuy_products"``

- ``python week1/index.py -s $BBUY_DATA``

- ``cd week1``
- ``pyenv activate search_eng``
