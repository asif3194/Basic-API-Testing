# Restful Booker API – Postman Collection

This repository contains a Postman Collection for interacting with the Restful Booker API. The collection includes complete CRUD operations for booking management, along with authentication.

---

## Features

### ✔ Create Booking  
Creates a new booking using customer details, booking dates, and additional needs.

### ✔ Get Booking  
Fetches booking details using a booking ID.

### ✔ Update Booking  
Updates an existing booking. Requires an authentication token.

### ✔ Access Token  
Generates an authentication token using admin credentials.

### ✔ Delete Booking  
Deletes a booking by ID using a valid authentication token.

---

## File Included

- **Basic.postman_collection.json** – Fully configured Postman Collection with requests, sample bodies, and endpoints.

---

## How to Use

### 1. Import into Postman
1. Open Postman  
2. Click **Import**  
3. Select `Basic.postman_collection.json`

### 2. Set Environment Variable

| Variable | Description |
|----------|-------------|
| `baseurl` | Base API URL (example: `https://restful-booker.herokuapp.com`) |

### 3. Execute Requests
Run the collection in this order:
1. **Access Token**
2. **Create Booking**
3. **Get Booking**
4. **Update Booking**
5. **Delete Booking**

---

## Example Request (Create Booking)

```json
{
  "firstname": "Asif",
  "lastname": "Rahman",
  "totalprice": 111,
  "depositpaid": true,
  "bookingdates": {
    "checkin": "2025-01-01",
    "checkout": "2025-02-01"
  },
  "additionalneeds": "Breakfast"
}
