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
    "name": "Ahmed"
}
```
Response => 
```
{
    "status": false,
    "reason": "user id is required!"
}
```

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 10' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d name=Ahmed http://127.0.0.1:4053/user/update
```
