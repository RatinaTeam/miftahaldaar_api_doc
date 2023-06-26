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
    "order_id": 1163
}
```
Response => 
```
{
    "status": true,
    "order": {
        "id": 1163,
        "emp_id": 1010,
        "supervisor_id": null,
        "order_type": "شراء",
        "customer_name": "sadsadsasad",
        "customer_phone": "5455555",
        "customer_salary_amount": "55555",
        "customer_salary_deposit_bank": "sdsad",
        "customer_employer": "asdsadsd",
        "customer_old": "20",
        "order_date": "2023-06-21 16:47:52",
        "status": "PENDING",
        "bank_name": "",
        "bank_employee_name": "ssssss",
        "duration": "",
        "mortgage": "",
        "personal_financing": "",
        "installment_amount": "",
        "premium_support": "",
        "type_of_property": "",
        "original_property_value": "",
        "customer_id": "",
        "owner_phone": "",
        "city_of_property": "",
        "property_value": "25000",
        "lead_source": "",
        "is_guarantees": null,
        "notes": "",
        "is_read": false,
        "attchemnets_json": "{\"صورة البطاقه\":\"/static/temporary/b325757b95cf4b5eb7e263e1763ca55a.png\",\"تعريف بالراتب\":\"\",\"برنت سمه\":\"\",\"كرت العائلة\":\"\",\"شهادة الاعفاء الضريبي\":\"\",\"بطاقة المالك\":\"\",\"صورة الصك\":\"\",\"رخصة البناء\":\"\",\"صورة التيار الكهربائي\":\"\",\"شهادة الاشغال\":\"\",\"الاقرار المساحي\":\"\",\"اتفاقية السعي\":\"\",\"صورة السند\":\"\",\"ابلكيشن البنك\":\"\",\"صورة من بطاقة المتضامن\":\"\",\"تعريف راتب المتضامن\":\"\",\"مرفق جديد\":\"/static/temporary/449d0c2d597346219ae88a9ebfa3d11e.png\"}",
        "evaluation_amount": "sssss",
        "paying_party": "asdadssad",
        "obligation_check": false,
        "delayed_until": null,
        "details_of_amount": "{}",
        "completed_percentage": 36.1702127659575,
        "last_update_note": "",
        "emp": {
            "id": 1010,
            "username": "admin"
        },
        "timeline": []
    }
}
```

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 13' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d order_id=1163 http://127.0.0.1:4053/order/get
```
