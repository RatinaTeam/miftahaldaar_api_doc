<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order_status/delay.md' mode='w+' encoding='utf-8'>
#OrderDelay# Request =>

POST /order_status/delay

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
    "notes": "Client is not responding",
    "delayed_until": "2023-05-29 11:18:07"
}
```
Response => 
```
b'<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">\n<title>500 Internal Server Error</title>\n<h1>Internal Server Error</h1>\n<p>The server encountered an internal error and was unable to complete your request.  Either the server is overloaded or there is an error in the application.</p>\n'

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 79' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: 18d78df6bf254dd4b9a2ad2a93f7144f' -H 'user-id: 1013' -d 'order_id=1&notes=Client+is+not+responding&delayed_until=2023-05-29+11%3A18%3A07' http://127.0.0.1:4053/order_status/delay
```
