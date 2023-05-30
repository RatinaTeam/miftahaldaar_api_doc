<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//orders/all.md' mode='w+' encoding='utf-8'>
#Get All Orders# Request =>

**GET** /orders/all?```id_index```=1

Headers Or Current SessionStore =>
```
{
    "user-id": "1013",
    "auth-key": "18d78df6bf254dd4b9a2ad2a93f7144f"
}
```
Response => 
```
{
    "status": true,
    "orders": [
        {
            "customer_name": "John Doe",
            "customer_phone": "123456789",
            "id": 1,
            "order_type": "Type A",
            "order_date": "2023-05-29 11:59:20",
            "status": "ON_PROGRESS",
            "bank_name": null,
            "customer_salary_amount": "5000",
            "last_update_note": null
        }
    ]
}
```

CURL command:
```
curl -X GET -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: 18d78df6bf254dd4b9a2ad2a93f7144f' -H 'user-id: 1013' 'http://127.0.0.1:4053/orders/all?id_index=1'
```
