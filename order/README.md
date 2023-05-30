`Order` class:

*   `id`: An integer field representing the unique identifier of the order.
*   `emp_id`: An integer field representing the employee ID associated with the order. It is used as an index.
*   `emp`: A property that returns the `UserAccount` object corresponding to the employee ID (`emp_id`).
*   `supervisor_id`: An integer field representing the supervisor ID associated with the order.
*   `supervisor`: A property that returns the `UserAccount` object corresponding to the supervisor ID (`supervisor_id`).
*   `order_type`: A string field representing the type of the order.
*   `customer_name`: A string field representing the name of the customer associated with the order.
*   `customer_phone`: A string field representing the phone number of the customer.
*   `customer_salary_amount`: A string field representing the amount of the customer's salary.
*   `customer_salary_deposit_bank`: A string field representing the bank where the customer's salary is deposited.
*   `customer_employer`: A string field representing the employer of the customer.
*   `customer_old`: A string field representing the age of the customer.
*   `order_date`: A DateTime field representing the date and time when the order was created. It has a default value of the current date and time and is indexed.
*   `status`: An enumeration field (`OrderStatus`) representing the status of the order. It has a default value of `OrderStatus.PENDING` and is indexed.
*   `bank_name`: A string field representing the name of the bank associated with the order.
*   `bank_employee_name`: A string field representing the name of the bank employee associated with the order.
*   `duration`: A string field representing the duration of the order.
*   `personal_financing`: A string field representing the personal financing information.
*   `installment_amount`: A string field representing the installment amount.
*   `premium_support`: A string field representing the premium support information.
*   `type_of_property`: A string field representing the type of the property.
*   `original_property_value`: A string field representing the original value of the property.
*   `customer_id`: A string field representing the customer's ID.
*   `owner_phone`: A string field representing the phone number of the property owner.
*   `city_of_property`: A string field representing the city where the property is located.
*   `property_value`: A string field representing the value of the property.
*   `lead_source`: A string field representing the source of the lead.
*   `is_guarantees`: A boolean field indicating whether guarantees are provided.
*   `notes`: A Text field representing additional notes about the order. It is nullable.
*   `is_read`: A boolean field indicating whether the order has been read.
*   `attachments_json`: A Text field representing the JSON data of the order's attachments. It is nullable and has a default value of `data.required_attachments_json`.
*   `evaluation_amount`: A string field representing the evaluation amount for the order. It is nullable.
*   `paying_party`: A string field representing the paying party information. It is nullable.
*   `obligation_check`: A boolean field indicating whether an obligation check has been performed. It has a default value of `False`.
*   `delayed_until`: A DateTime field representing the date and time until which the order is delayed. It is nullable.
*   `details_of_amount`: A Text field representing the details of the amount for the order. It is nullable and has a default value of '\[\]'.
*   `completed_percentage`: A Float field representing the percentage of completion for the order. It has a default value of `0`.
*   `last_update_note`: A Text field representing the last update note

`/order/<action>` endpoint:

1.  **Create**:
    
    *   The endpoint receives the form data containing the required fields for creating a new order.
    *   It creates a new instance of the `Order` model.
    *   It populates the instance with the provided form data.
    *   The order is saved to the database.
    *   An entry is created in the `OrderTimeline` to track the registration of the order.
    *   A success response is returned with a message indicating the successful creation of the order.
2.  **Update**:
    
    *   The endpoint receives the form data containing the order ID and the fields to update.
    *   It retrieves the existing order from the database based on the provided order ID.
    *   It checks if the user is authorized to update the order.
    *   It updates the order instance with the provided form data.
    *   The order is updated in the database.
    *   A success response is returned with a message indicating the successful update of the order.
3.  **Get**:
    
    *   The endpoint receives the order ID from the form data.
    *   It retrieves the order from the database based on the provided order ID.
    *   It checks if the user is authorized to access the order.
    *   The order details are returned as a response.
4.  **Register**:
    
    *   The endpoint receives the form data containing the required fields for registering a new order.
    *   It creates a new instance of the `Order` model.
    *   It populates the instance with the provided form data.
    *   The order is saved to the database.
    *   An entry is created in the `OrderTimeline` to track the registration of the order.
    *   A success response is returned with a message indicating the successful registration of the order.
5.  **Delete**:
    
    *   The endpoint receives the order ID from the form data.
    *   It retrieves the existing order from the database based on the provided order ID.
    *   It checks if the user is authorized to delete the order.
    *   The order is deleted from the database.
    *   A success response is returned with a message indicating the successful deletion of the order.

Please note that the backend implementation may involve additional logic and database operations specific to your application's requirements. The provided explanation gives a high-level overview of the actions performed in each scenario.

If you have any further questions, feel free to ask!
