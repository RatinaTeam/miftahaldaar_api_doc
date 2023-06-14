<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//orders/delayed_orders.md' mode='w+' encoding='utf-8'>
#Get Delayed Orders# Request =>

**GET** /orders/delayed_orders

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
    "orders": [
        {
            "customer_name": "John Doe",
            "customer_phone": "123456789",
            "id": 1,
            "order_type": "Type A",
            "order_date": "2023-05-29 11:59:20",
            "status": "DELAYED",
            "bank_name": null,
            "customer_salary_amount": "5000",
            "last_update_note": "Client is not responding",
            "completed_percentage": 63.8297872340426,
            "emp_id": 1010,
            "emp": {
                "id": 1010,
                "username": "admin"
            }
        }
    ]
}
```

CURL command =>
```
curl -X GET -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' http://127.0.0.1:4053/orders/delayed_orders
```
