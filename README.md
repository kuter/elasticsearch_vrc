# elasticsearch_vrc

## Importing test data with cURL

curl -H "Content-Type: application/json" -XPOST "http://localhost:9200/product/_doc/_bulk?pretty" --data-binary "@products.json"
curl -H "Content-Type: application/json" -XPOST "http://localhost:9200/recipe/_doc/_bulk?pretty" --data-binary "@recipes.json"
curl -H "Content-Type: application/json" -XPOST 'http://localhost:9200/order/_doc/_bulk?pretty' --data-binary "@orders-bulk.json"
