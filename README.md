## Neural Collaborative Filtering (NCF) Model for Enhanced Sales and Customer Satisfaction

This recommendation system utilizes Neural Collaborative Filtering (NCF) to provide highly personalized product suggestions. By analyzing user behavior and preferences, the model can identify patterns and correlations that enable it to recommend items that are most likely to be purchased or appreciated by customers.

---

## Data Attributes

### **orders_df**
- **order_id**: Unique identifier for each order placed on the e-commerce platform.
- **customer_id**: Unique identifier for each customer who made a transaction.
- **order_status**: The status of the order.
- **order_purchase_timestamp**: The exact time and date when the order was placed by the customer.
- **order_approved_at**: The exact time and date when the payment for the order was approved by the system.
- **order_delivered_carrier_date**: The exact time and date when the product was handed over to the shipping carrier for further processing.
- **order_delivered_customer_date**: The exact time and date when the order was received by the customer.
- **order_estimated_delivery_date**: The estimated delivery date of the order to the customer as provided by the system.

### **customers_df**
- **customer_id**: Unique identifier for each customer who made a transaction.
- **customer_unique_id**: Unique identifier for the customer, typically used to track the customer's transactions within the system.
- **customer_zip_code_prefix**: The postal code indicating the customer's geographical location.
- **customer_city**: The name of the city where the customer resides.
- **customer_state**: The name of the state where the customer resides.

### **sellers_df**
- **seller_id**: Unique identifier for the seller.
- **seller_zip_code_prefix**: The postal code indicating the seller's geographical location.
- **seller_city**: The name of the city where the seller operates.
- **seller_state**: The name of the state where the seller operates.

### **products_df**
- **product_id**: Unique identifier for the product being sold.
- **product_category_name**: The category of the product being sold, such as electronics, clothing, or household appliances.
- **product_name_length**: The length of the product name in characters.
- **product_description_length**: The length of the product description in characters.
- **product_photos_qty**: The number of product photos provided by the seller in the product listing.
- **product_weight_g**: The weight of the product in grams.
- **product_length_cm**: The length of the product in centimeters.
- **product_height_cm**: The height of the product in centimeters.
- **product_width_cm**: The width of the product in centimeters.

### **geolocation_df**
- **geolocation_zip_code_prefix**: Zip code prefix or a portion of the full zip code that indicates the geographic location.
- **geolocation_lat**: Latitude geographic coordinate indicating the north or south position relative to the equator.
- **geolocation_lng**: Longitude geographic coordinate indicating the east or west position relative to the Prime Meridian (Greenwich).
- **geolocation_city**: The name of the city where the location is situated.
- **geolocation_state**: The state or province abbreviation where the location is situated.

### **order_items_df**
- **order_id**: Unique identifier for each order placed on the e-commerce platform.
- **order_item_id**: Unique identifier for an item within an order, often used to identify multiple items within a single order.
- **shipping_limit_date**: The deadline for the seller to ship the product as per the agreement.
- **price**: The price of the product sold on the e-commerce platform.
- **freight_value**: The shipping cost of the product from the seller to the customer.
- **product_id**: Unique identifier for the product being sold.
- **seller_id**: Unique identifier for the seller.

### **order_payments_df**
- **order_id**: Unique identifier for each order placed on the e-commerce platform.
- **payment_sequential**: The sequence of payment transactions, useful if there are multiple payments within a single transaction.
- **payment_type**: The type of payment used by the customer, such as credit card, bank transfer, or cash on delivery.
- **payment_installments**: The number of installments for the payment if the customer chose a split payment option.
- **payment_value**: The total value of the payment made by the customer for the transaction.

### **order_reviews_df**
- **order_id**: Unique identifier for each order placed on the e-commerce platform.
- **review_id**: Unique identifier for each review given by the customer.
- **review_score**: The review score given by the customer, typically ranging from 1 to 5, indicating the customer's satisfaction level.
- **review_comment_title**: The title of the comment or review given by the customer.
- **review_comment_message**: The content or message of the review given by the customer.
- **review_creation_date**: The date and time when the review was created by the customer.
- **review_answer_timestamp**: The time and date when the seller or platform responded to the review given by the customer.
- **response_time**: The time taken by the seller or platform to respond to the customer's review or inquiry.
