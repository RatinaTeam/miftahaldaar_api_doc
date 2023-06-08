<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order/create.md' mode='w+' encoding='utf-8'>
#CreateOrder# Request =>

POST /order/create

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
    "order_type": "Type S",
    "customer_name": "Khalid",
    "customer_phone": "0555555555",
    "customer_salary_amount": "5000",
    "customer_salary_deposit_bank": "HSBC Bank",
    "customer_employer": "XYZ Company",
    "customer_old": "30",
    "bank_employee_name": "Jane Smith",
    "property_value": "250000"
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
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 229' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d 'order_type=Type+S&customer_name=Khalid&customer_phone=0555555555&customer_salary_amount=5000&customer_salary_deposit_bank=HSBC+Bank&customer_employer=XYZ+Company&customer_old=30&bank_employee_name=Jane+Smith&property_value=250000' http://127.0.0.1:4053/order/create
```
