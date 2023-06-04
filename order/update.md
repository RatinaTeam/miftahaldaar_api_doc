<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order/update.md' mode='w+' encoding='utf-8'>
#UpdateOrder# Request =>

POST /order/update

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
    "order_id": 1,
    "attchemnets_json": "{\"\\u0635\\u0648\\u0631\\u0629 \\u0627\\u0644\\u0628\\u0637\\u0627\\u0642\\u0647\": \"https://liteamay.nyc3.digitaloceanspaces.com/2021/04/resize.jpg\"}"
}
```
Response => 
```
{
    "status": true
}
```

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 214' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: 18d78df6bf254dd4b9a2ad2a93f7144f' -H 'user-id: 1013' -d 'order_id=1&attchemnets_json=%7B%22%5Cu0635%5Cu0648%5Cu0631%5Cu0629+%5Cu0627%5Cu0644%5Cu0628%5Cu0637%5Cu0627%5Cu0642%5Cu0647%22%3A+%22https%3A%2F%2Fliteamay.nyc3.digitaloceanspaces.com%2F2021%2F04%2Fresize.jpg%22%7D' http://127.0.0.1:4053/order/update
```
