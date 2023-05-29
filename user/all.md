<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//user/all.md' mode='w+' encoding='utf-8'>
#Get All Users# Request =>

**GET** /user/all

Headers =>
```
{
    "user-id": "1010",
    "auth-key": "sdofmasdmfasdmflkmasdf"
}
```
Response =>
```
{
    "status": true,
    "users": [
        {
            "id": 1010,
            "username": "admin",
            "is_active": true,
            "role": "ADMIN"
        },
        {
            "id": 1012,
            "username": "احمد",
            "is_active": false,
            "role": "EMPLOYEE"
        }
    ]
}
```

CURL command =>
```
curl -X GET -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' http://127.0.0.1:4053/user/all
```
