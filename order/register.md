<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order/register.md' mode='w+' encoding='utf-8'>
#Register order# Request =>

POST /order/register

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
    "action": "register",
    "order_type": "Type A",
    "customer_name": "John Doe",
    "customer_phone": "123456789",
    "customer_salary_amount": "5000",
    "customer_salary_deposit_bank": "ABC Bank",
    "customer_employer": "XYZ Company",
    "customer_old": "30",
    "bank_employee_name": "Jane Smith",
    "property_value": "250000"
}
```
Response => 
```
b'<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">\n<title>500 Internal Server Error</title>\n<h1>Internal Server Error</h1>\n<p>The server encountered an internal error and was unable to complete your request.  Either the server is overloaded or there is an error in the application.</p>\n'

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 245' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: sdofmasdmfasdmflkmasdf' -H 'user-id: 1010' -d 'action=register&order_type=Type+A&customer_name=John+Doe&customer_phone=123456789&customer_salary_amount=5000&customer_salary_deposit_bank=ABC+Bank&customer_employer=XYZ+Company&customer_old=30&bank_employee_name=Jane+Smith&property_value=250000' http://127.0.0.1:4053/order/register
```
