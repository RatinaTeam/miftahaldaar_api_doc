<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//user/create.md' mode='w+' encoding='utf-8'>
#CreateUser# Request =>

POST /user/create

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
    "username": "احمد",
    "password": "12233",
    "is_active": true,
    "role": "EMPLOYEE"
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
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 77' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d 'username=%D8%A7%D8%AD%D9%85%D8%AF&password=12233&is_active=True&role=EMPLOYEE' http://127.0.0.1:4053/user/create
```
