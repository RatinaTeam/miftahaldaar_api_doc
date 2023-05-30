Certainly! Here's the full message you provided formatted in markdown:

sql
Copy code
## `/order_status/<action>` Method: POST

**Description:** This endpoint is used to update the status of an order. The available actions are 'update', 'assign', 'delay', 'add_notes', and 'read'.

**Parameters:**

- `action` (string, path parameter): Specifies the action to be performed on the order status.
- `status` (string, request parameter): Specifies the new status for the order. Valid values are 'ON_PROGRESS', 'DELAYED', 'PARTIALLY_COMPLETED', and 'COMPLETED'.
- `order_id` (integer, request parameter): Specifies the ID of the order to be updated.
- `notes` (string, request parameter): Optional. Additional notes or comments regarding the order status.
- `delayed_date` (string, request parameter): Optional. Specifies the delayed date in the format 'YYYY-MM-DD' if the status is 'DELAYED'.

**Response:**

The response will be a JSON object with the following fields:

- `success` (boolean): Indicates whether the request was successful or not.
- `message` (string): Provides a descriptive message regarding the status of the request.

**Authorization:**

The user making the request must be authenticated and authorized based on their role and the order's assigned employee ID.

### Examples:

#### Update Order Status

**Request:**

POST /order_status/update
Content-Type: application/json
```
{
"status": "COMPLETED",
"order_id": 12345
}
```


**Response:**
```
{
"success": true,
"message": "Order status updated successfully!"
}
```


#### Assign Order to Employee

**Request:**
```
POST /order_status/assign
Content-Type: application/json
```
```
{
"emp_id": 9876,
"order_id": 12345
}
```



**Response:**
```
{
"success": true,
"message": "Order assigned to employee successfully!"
}
```







