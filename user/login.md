<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//user/login.md' mode='w+' encoding='utf-8'>
#Restaurant info# Request =>

POST /user/login

Headers Or Current SessionStore =>
```
{}
```
Body => 
```
{
    "uid": 1010,
    "password": "password123"
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
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 29' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -d 'uid=1010&password=password123' http://127.0.0.1:4053/user/login
```
