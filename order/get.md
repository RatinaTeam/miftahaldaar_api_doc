<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order/get.md' mode='w+' encoding='utf-8'>
#GetOrder# Request =>

**GET** /order/get?```order_id```=1

Headers Or Current SessionStore =>
```
{
    "user-id": "1013",
    "auth-key": "18d78df6bf254dd4b9a2ad2a93f7144f"
}
```
Response => 
```
b'<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">\n<title>405 Method Not Allowed</title>\n<h1>Method Not Allowed</h1>\n<p>The method is not allowed for the requested URL.</p>\n'

CURL command:
```
curl -X GET -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: 18d78df6bf254dd4b9a2ad2a93f7144f' -H 'user-id: 1013' 'http://127.0.0.1:4053/order/get?order_id=1'
```
