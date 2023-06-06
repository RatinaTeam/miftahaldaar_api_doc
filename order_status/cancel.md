<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order_status/cancel.md' mode='w+' encoding='utf-8'>
#OrderCancel# Request =>

POST /order_status/cancel

Headers Or Current SessionStore =>
```
{
    "user-id": "1013",
    "auth-key": "18d78df6bf254dd4b9a2ad2a93f7144f"
}
```
Body => 
```
{
    "order_id": 1013,
    "notes": "Client is not responding"
}
```
Response => 
```
{
    "status": true,
    "order_status": "CANCELLED",
    "order_id": 1013
}
```

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 44' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: 18d78df6bf254dd4b9a2ad2a93f7144f' -H 'user-id: 1013' -d 'order_id=1013&notes=Client+is+not+responding' http://127.0.0.1:4053/order_status/cancel
```
