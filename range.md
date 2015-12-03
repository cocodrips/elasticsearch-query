
## 1000以上
```json
{
    "fields": ["score"],
    "query": {
        "range": {
            "score": {
                "gte": 1000
            }
        }
    }
}
```

## curl
```sh
curl -XGET http://localhost:9200/index/type/_search?pretty -s '
{
    "fields": ["score"],
    "query": {
        "range": {
            "score": {
                "gte": 1000
            }
        }
    }
}
'

```
