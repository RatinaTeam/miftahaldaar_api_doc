<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//user/logout.md' mode='w+' encoding='utf-8'>
#Logout# Request =>

POST/user/logout

Headers =>
```
{
    "user-id": "1826",
    "auth-key": "sdofmasdmfasdmflkmasdf"
}
```
Body =>
```
{}
```
Response =>
```
{
    "status": true
}
```

CURL command =>
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 0' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1826' http://127.0.0.1:4053/user/logout
```
