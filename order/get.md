<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order/get.md' mode='w+' encoding='utf-8'>
#GetOrder# Request =>

POST /order/get

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
    "order_id": 1
}
```
Response => 
```
{
    "status": true,
    "order": {
        "id": 1,
        "emp_id": 1010,
        "supervisor_id": null,
        "order_type": "Type A",
        "customer_name": "John Doe",
        "customer_phone": "123456789",
        "customer_salary_amount": "5000",
        "customer_salary_deposit_bank": "ABC Bank",
        "customer_employer": "XYZ Company",
        "customer_old": "30",
        "order_date": "2023-05-29 11:59:20",
        "status": "DELAYED",
        "bank_name": null,
        "bank_employee_name": "Jane Smith",
        "duration": null,
        "mortgage": null,
        "personal_financing": null,
        "installment_amount": null,
        "premium_support": null,
        "type_of_property": null,
        "original_property_value": null,
        "customer_id": null,
        "owner_phone": null,
        "city_of_property": null,
        "property_value": "250000",
        "lead_source": null,
        "is_guarantees": null,
        "notes": null,
        "is_read": false,
        "attchemnets_json": "{\"\\u0635\\u0648\\u0631\\u0629 \\u0627\\u0644\\u0628\\u0637\\u0627\\u0642\\u0647\": \"https://liteamay.nyc3.digitaloceanspaces.com/2021/04/resize.jpg\"}",
        "evaluation_amount": null,
        "paying_party": null,
        "obligation_check": false,
        "delayed_until": "2023-05-29 11:18:07",
        "details_of_amount": "[]",
        "completed_percentage": 63.8297872340426,
        "last_update_note": "Client is not responding",
        "emp": {
            "id": 1010,
            "username": "admin"
        },
        "timeline": [
            {
                "id": 19,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "This is a note",
                "created_at": "2023-05-30 11:18:07"
            },
            {
                "id": 21,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "Client is not responding",
                "created_at": "2023-05-30 11:18:07"
            },
            {
                "id": 22,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "Client is not responding",
                "created_at": "2023-05-30 11:18:07"
            },
            {
                "id": 23,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "Client is not responding",
                "created_at": "2023-05-30 11:34:16"
            },
            {
                "id": 24,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "Client is not responding",
                "created_at": "2023-05-30 11:41:28"
            },
            {
                "id": 25,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "Client is not responding",
                "created_at": "2023-05-30 12:00:57"
            },
            {
                "id": 26,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "Client is not responding",
                "created_at": "2023-05-30 12:01:15"
            },
            {
                "id": 27,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "Client is not responding",
                "created_at": "2023-05-30 12:06:05"
            },
            {
                "id": 28,
                "order_id": 1,
                "emp_id": 1013,
                "status": "ON_PROGRESS",
                "notes": "Client is not responding",
                "created_at": "2023-05-30 12:07:58"
            },
            {
                "id": 57,
                "order_id": 1,
                "emp_id": 1010,
                "status": "PENDING",
                "notes": "responded",
                "created_at": "2023-06-10 10:51:48"
            }
        ]
    }
}
```

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 10' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d order_id=1 http://127.0.0.1:4053/order/get
```
