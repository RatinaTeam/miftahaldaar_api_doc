<_io.TextIOWrapper name='/root/miftahaldaar_api_doc//order_status/add_notes.md' mode='w+' encoding='utf-8'>
#OrderAddNotes# Request =>

POST /order_status/add_notes

Headers Or Current SessionStore =>
```
{
    "user-id": "1013",
    "auth-key": "18d78df6bf254dd4b9a2ad2a93f7144f"
}
```
Body => 
```
{
    "order_id": 1,
    "note": "This is a note"
}
```
Response => 
```
{
    "status": true,
    "order": {
        "id": 1,
        "emp_id": 1013,
        "supervisor_id": null,
        "order_type": "Type A",
        "customer_name": "John Doe",
        "customer_phone": "123456789",
        "customer_salary_amount": "5000",
        "customer_salary_deposit_bank": "ABC Bank",
        "customer_employer": "XYZ Company",
        "customer_old": "30",
        "order_date": "2023-05-29 11:59:20",
        "status": "ON_PROGRESS",
        "bank_name": null,
        "bank_employee_name": "Jane Smith",
        "duration": null,
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
        "attchemnets_json": "{\"\\u0635\\u0648\\u0631\\u0629 \\u0627\\u0644\\u0628\\u0637\\u0627\\u0642\\u0647\": \"\", \"\\u062a\\u0639\\u0631\\u064a\\u0641 \\u0628\\u0627\\u0644\\u0631\\u0627\\u062a\\u0628\": \"\", \"\\u0628\\u0631\\u0646\\u062a \\u0633\\u0645\\u0647\": \"\", \"\\u0643\\u0631\\u062a \\u0627\\u0644\\u0639\\u0627\\u0626\\u0644\\u0629\": \"\", \"\\u0634\\u0647\\u0627\\u062f\\u0629 \\u0627\\u0644\\u0627\\u0639\\u0641\\u0627\\u0621 \\u0627\\u0644\\u0636\\u0631\\u064a\\u0628\\u064a\": \"\", \"\\u0628\\u0637\\u0627\\u0642\\u0629 \\u0627\\u0644\\u0645\\u0627\\u0644\\u0643\": \"\", \"\\u0635\\u0648\\u0631\\u0629 \\u0627\\u0644\\u0635\\u0643\": \"\", \"\\u0631\\u062e\\u0635\\u0629 \\u0627\\u0644\\u0628\\u0646\\u0627\\u0621\": \"\", \"\\u0635\\u0648\\u0631\\u0629 \\u0627\\u0644\\u062a\\u064a\\u0627\\u0631 \\u0627\\u0644\\u0643\\u0647\\u0631\\u0628\\u0627\\u0626\\u064a\": \"\", \"\\u0634\\u0647\\u0627\\u062f\\u0629 \\u0627\\u0644\\u0627\\u0634\\u063a\\u0627\\u0644\": \"\", \"\\u0627\\u0644\\u0627\\u0642\\u0631\\u0627\\u0631 \\u0627\\u0644\\u0645\\u0633\\u0627\\u062d\\u064a\": \"\", \"\\u0627\\u062a\\u0641\\u0627\\u0642\\u064a\\u0629 \\u0627\\u0644\\u0633\\u0639\\u064a\": \"\", \"\\u0635\\u0648\\u0631\\u0629 \\u0627\\u0644\\u0633\\u0646\\u062f\": \"\", \"\\u0627\\u0628\\u0644\\u0643\\u064a\\u0634\\u0646 \\u0627\\u0644\\u0628\\u0646\\u0643\": \"\", \"\\u0635\\u0648\\u0631\\u0629 \\u0645\\u0646 \\u0628\\u0637\\u0627\\u0642\\u0629 \\u0627\\u0644\\u0645\\u062a\\u0636\\u0627\\u0645\\u0646\": \"\", \"\\u062a\\u0639\\u0631\\u064a\\u0641 \\u0631\\u0627\\u062a\\u0628 \\u0627\\u0644\\u0645\\u062a\\u0636\\u0627\\u0645\\u0646\": \"\"}",
        "evaluation_amount": null,
        "paying_party": null,
        "obligation_check": false,
        "delayed_until": null,
        "details_of_amount": "[]",
        "completed_percentage": 30.4347826086957,
        "last_update_note": null
    }
}
```

CURL command:
```
curl -X POST -H 'Accept: */*' -H 'Accept-Encoding: gzip, deflate' -H 'Connection: keep-alive' -H 'Content-Length: 30' -H 'Content-Type: application/x-www-form-urlencoded' -H 'User-Agent: python-requests/2.18.4' -H 'auth-key: 18d78df6bf254dd4b9a2ad2a93f7144f' -H 'user-id: 1013' -d 'order_id=1&note=This+is+a+note' http://127.0.0.1:4053/order_status/add_notes
```
