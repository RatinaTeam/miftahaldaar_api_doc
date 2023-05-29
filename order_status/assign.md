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
b'<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">\n<title>500 Internal Server Error</title>\n<h1>Internal Server Error</h1>\n<p>The server encountered an internal error and was unable to complete your request.  Either the server is overloaded or there is an error in the application.</p>\n'

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 22' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d 'order_id=1&emp_id=1013' http://127.0.0.1:4053/order_status/assign
```
