<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//user/update.md' mode='w+' encoding='utf-8'>
#UserUpdate# Request =>

POST /user/update

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
    "id": 1012,
    "name": "Ahmed"
}
```
Response => 
```
{
    "status": false,
    "reason": "role is not valid!"
}
```

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 18' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d 'id=1012&name=Ahmed' http://127.0.0.1:4053/user/update
```
