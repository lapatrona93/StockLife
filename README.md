
# StockLife

StockLife is an intuitive software tool designed to streamline the management of product expiry dates. It helps businesses, retailers, and warehouses keep track of inventory to ensure that products are sold or used before they expire. With automated alerts and real-time monitoring, StockLife reduces the risk of waste, improves product turnover, and enhances inventory accuracy. Whether you're managing perishable goods, pharmaceuticals, or any other time-sensitive products, StockLife offers an efficient solution to safeguard quality, meet compliance standards, and optimize stock management.




## Requirements
**User Registration & Authentication:**

- Secure user registration with email and password.
- Login and logout functionality.
- Password reset option.

**Product Management:**

- Add new products/barcode with fields like product name, category, and barcode.
- Update product details, such as name, category, and quantity
- Remove or deactivate outdated or discontinued products.


**Expiry Date Management:**

- Display expiry dates for products based on their barcode
- Automatic alerts for products nearing expiry.
- Option to sort inventory based on expiry dates.

**User Roles & Permissions:**

- Define roles such as Admin, Manager, and Staff with specific permissions.
- Allow different levels of access for each role.


**Search & Filter:**

- Quick search option for products by name or barcode.
- Advanced filters to narrow down inventory by category and expiry.


**Audit Logs:**

- Track and log every action performed within the software.



## API Reference

#### 1. Register a new product/barcode
- **Endpoint**: POST /api/products
- **Description** : Add a new barcode/product to inventory based on its barcode
- **Request Body(JSON)**:

  ```http
  {
    "barcode": "1234567890",
    "name": "Product A",
    "description": "test test",
    "Unit": "100ml",
    "distributor": "Distributor XYZ",
    "invoice_number": "INV12345",
    "invoice_date": "2024-11-13",
    "expiry_date": "2025-11-13",
    "quantity": 100
  }     

- **Response**:
    ```http
  {
        "id": 1,
        "barcode": "1234567890",
        "name": "Product A",
        "description": "test test",
        "Unit": "100ml",
        "distributor": "Distributor XYZ",
        "invoice_number": "INV12345",
        "invoice_date": "2024-11-13",
        "expiry_date": "2025-11-13",
        "quantity": 100,
        "days_to_expire": 365
    }



#### 2. Retrieve a product
- **Endpoint**: POST /api/products
- **Description** : Add a new barcode/product to inventory based on its barcode
- **Request Body(JSON)**:

  ```http
  {
    "barcode": "1234567890",
    "name": "Product A",
    "description": "test test",
    "Unit": "100ml",
    "distributor": "Distributor XYZ",
    "invoice_number": "INV12345",
    "invoice_date": "2024-11-13",
    "expiry_date": "2025-11-13",
    "quantity": 100
  }     

- **Response**:
    ```http
  {
        "id": 1,
        "barcode": "1234567890",
        "name": "Product A",
        "description": "test test",
        "Unit": "100ml",
        "distributor": "Distributor XYZ",
        "invoice_number": "INV12345",
        "invoice_date": "2024-11-13",
        "expiry_date": "2025-11-13",
        "quantity": 100,
        "days_to_expire": 365
    }


#### 3. Retrieve all products
- **Endpoint**: POST /api/products
- **Description** : Add a new barcode/product to inventory based on its barcode
- **Request Body(JSON)**:

  ```http
  {
    "barcode": "1234567890",
    "name": "Product A",
    "description": "test test",
    "Unit": "100ml",
    "distributor": "Distributor XYZ",
    "invoice_number": "INV12345",
    "invoice_date": "2024-11-13",
    "expiry_date": "2025-11-13",
    "quantity": 100
  }     

- **Response**:
    ```http
  {
        "id": 1,
        "barcode": "1234567890",
        "name": "Product A",
        "description": "test test",
        "Unit": "100ml",
        "distributor": "Distributor XYZ",
        "invoice_number": "INV12345",
        "invoice_date": "2024-11-13",
        "expiry_date": "2025-11-13",
        "quantity": 100,
        "days_to_expire": 365
    }


#### 4. Register a new Distributor
- **Endpoint**: POST /api/products
- **Description** : Add a new barcode/product to inventory based on its barcode
- **Request Body(JSON)**:

  ```http
  {
    "barcode": "1234567890",
    "name": "Product A",
    "description": "test test",
    "Unit": "100ml",
    "distributor": "Distributor XYZ",
    "invoice_number": "INV12345",
    "invoice_date": "2024-11-13",
    "expiry_date": "2025-11-13",
    "quantity": 100
  }     

- **Response**:
    ```http
  {
        "id": 1,
        "barcode": "1234567890",
        "name": "Product A",
        "description": "test test",
        "Unit": "100ml",
        "distributor": "Distributor XYZ",
        "invoice_number": "INV12345",
        "invoice_date": "2024-11-13",
        "expiry_date": "2025-11-13",
        "quantity": 100,
        "days_to_expire": 365
    }


#### 5. Retrieve a Distributor
- **Endpoint**: POST /api/products
- **Description** : Add a new barcode/product to inventory based on its barcode
- **Request Body(JSON)**:

  ```http
  {
    "barcode": "1234567890",
    "name": "Product A",
    "description": "test test",
    "Unit": "100ml",
    "distributor": "Distributor XYZ",
    "invoice_number": "INV12345",
    "invoice_date": "2024-11-13",
    "expiry_date": "2025-11-13",
    "quantity": 100
  }     

- **Response**:
    ```http
  {
        "id": 1,
        "barcode": "1234567890",
        "name": "Product A",
        "description": "test test",
        "Unit": "100ml",
        "distributor": "Distributor XYZ",
        "invoice_number": "INV12345",
        "invoice_date": "2024-11-13",
        "expiry_date": "2025-11-13",
        "quantity": 100,
        "days_to_expire": 365
    }


#### 6. Retrieve all Distributors
- **Endpoint**: POST /api/products
- **Description** : Add a new barcode/product to inventory based on its barcode
- **Request Body(JSON)**:

  ```http
  {
    "barcode": "1234567890",
    "name": "Product A",
    "description": "test test",
    "Unit": "100ml",
    "distributor": "Distributor XYZ",
    "invoice_number": "INV12345",
    "invoice_date": "2024-11-13",
    "expiry_date": "2025-11-13",
    "quantity": 100
  }     

- **Response**:
    ```http
  {
        "id": 1,
        "barcode": "1234567890",
        "name": "Product A",
        "description": "test test",
        "Unit": "100ml",
        "distributor": "Distributor XYZ",
        "invoice_number": "INV12345",
        "invoice_date": "2024-11-13",
        "expiry_date": "2025-11-13",
        "quantity": 100,
        "days_to_expire": 365
    }
## Database & Tables

#### Product
- **barcode:** string, required
- **name:** string, required
- **description:** string, required
- **unit:** string, required
- **distributor:** string, required
- **invoice_number:** string, required
- **invoice_date:** ISO Date, required
- **expiry_date:** ISO Date, required
- **quanty:** Integer, required
- **days_to_expire:** Integer, required


#### Ditributor
- **name:** string, required
- **address:** string, required
- **phone_number:** string, required
- **email:** string, required


#### User
- **email:** string, required
- **password:** string, required
- **first_name:** string, required
- **last_name:** string, required
