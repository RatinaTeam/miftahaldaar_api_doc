Sure! Here's the documentation for the `/orders/<page>` endpoint:

Get Orders
----------

Retrieves a list of orders based on the specified page and query parameters.

### Endpoint

bashCopy code

`GET /orders/<page>`

### Parameters

*   `<page>` (string): The page of orders to retrieve. Possible values:
    *   `"new_orders"`: Retrieves new orders for the current user.
    *   `"all_orders"`: Retrieves all orders for the current user.
    *   `"delayed_orders"`: Retrieves delayed orders for the current user.

### Query Parameters

The endpoint accepts the following query parameters to filter the orders:

*   `customer_name` (string): Filters orders by customer name.
*   `customer_phone` (string): Filters orders by customer phone number.
*   `id` (integer): Filters orders by order ID.
*   `order_type` (string): Filters orders by order type.
*   `order_date` (string): Filters orders by order date.
*   `status` (string): Filters orders by status.
*   `bank_name` (string): Filters orders by bank name.
*   `customer_salary_amount` (string): Filters orders by customer salary amount.
*   `last_update_note` (string): Filters orders by last update note.

### Response

The endpoint returns a JSON response with the following structure:

jsonCopy code

```
{
   "success":true,
   "orders":[
      {
         "customer_name":"John Doe",
         "customer_phone":"123456789",
         "id":1,
         "order_type":"Type A",
         "order_date":"2023-05-29 10:30:00",
         "status":"pending",
         "bank_name":"ABC Bank",
         "customer_salary_amount":"5000",
         "last_update_note":"Updated note"
      },
      {
         "customer_name":"Jane Smith",
         "customer_phone":"987654321",
         "id":2,
         "order_type":"Type B",
         "order_date":"2023-05-28 14:45:00",
         "status":"completed",
         "bank_name":"XYZ Bank",
         "customer_salary_amount":"8000",
         "last_update_note":"Another note"
      },
      "..."
   ]
}
```

*   `success` (boolean): Indicates if the request was successful.
*   `orders` (array): An array of order objects matching the query parameters. Each order object contains the selected fields from the `Order.search_fields` list.

### Authorization

The endpoint requires authentication to access. The user making the request must be logged in with valid credentials.

### Examples

1.  Retrieve new orders for the current user:



`GET /orders/new_orders`

2.  Retrieve all orders for the current user:

`GET /orders/all_orders`

3.  Retrieve delayed orders for the current user:



```GET /orders/delayed_orders```

4.  Retrieve orders filtered by customer name and order type:



`GET /orders/all_orders?customer_name=John Doe&order_type=Type A`

5.  Retrieve orders filtered by status and bank name:

bashCopy code

`GET /orders/all_orders?status=completed&bank_name=ABC Bank`

Please note that the endpoint may require additional configuration and implementation based on your specific environment and database setup.

Let me know if there's anything else I can assist you with!
