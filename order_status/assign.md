<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order_status/assign.md' mode='w+' encoding='utf-8'>
#Order assign# Request =>

POST /order_status/assign

Headers Or Current SessionStore =>
```
{
    "user-id": "1010",
    "auth-key": "sdofmasdmfasdmflkmasdf"
}
```
Body => 
```
{
    "order_id": 1,
    "emp_id": 1013
}
```
Response => 
```
{
    "status": true,
    "order": null
}
```

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 22' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d 'order_id=1&emp_id=1013' http://127.0.0.1:4053/order_status/assign
```
