# 🚀 **AutomationExercise API Testing**

![Postman](https://img.shields.io/badge/Postman-Collection-orange?style=flat-square)
![API](https://img.shields.io/badge/API-Test-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-success?style=flat-square)

## 🌟 **Overview**

This project contains a Postman collection for testing the API endpoints provided by [AutomationExercise](https://www.automationexercise.com/). It includes multiple test scenarios to validate the functionality, responses, and performance of the API.

---

## 📦 **Collection Summary**

### 🔑 **Endpoints Covered:**

1. **Products API:**
   - `GET /api/productsList` - Retrieve all products.
   - `POST /api/productsList` - Validate unsupported method.

2. **Brands API:**
   - `GET /api/brandsList` - Fetch all brands.
   - `PUT /api/brandsList` - Validate unsupported method.

3. **Search API:**
   - `POST /api/searchProduct` - Search for a product.
   - `POST /api/searchProduct` (without parameter) - Error scenario.

4. **User Account API:**
   - `POST /api/createAccount` - Create a new user.
   - `DELETE /api/deleteAccount` - Remove an account.
   - `PUT /api/updateAccount` - Update user details.
   - `GET /api/getUserDetailByEmail` - Fetch user details by email.

5. **Login API:**
   - `POST /api/verifyLogin` - Verify login with valid and invalid details.

---

## 🧪 **Tests Included**

Each endpoint has associated Postman tests to ensure proper functionality:

✅ **Status Code Checks:** Ensure the expected HTTP status codes are returned.

📝 **Response Validation:** Verify the structure and data types of the JSON responses.

⚙️ **Performance Testing:** Ensure responses are returned within acceptable time limits (< 1s).

🚫 **Error Handling:** Validate correct error messages for invalid requests.

---

## 🚀 **Getting Started**

1. Install [Postman](https://www.postman.com/downloads/).
2. Clone the repository:

```bash
git clone https://github.com/yourusername/automation-exercise-api-testing.git
```

3. Import the Postman collection (`AutomationExercise.com.postman_collection.json`) into Postman.
4. Set the `{{base_url}}` environment variable to `https://automationexercise.com`.
5. Run the collection and view results.

---

## 📜 **Example Request & Response**

**GET /api/productsList**

**Request:**
```http
GET {{base_url}}/api/productsList
```

**Response:**
```json
{
  "responseCode": 200,
  "products": [
    {
      "id": 1,
      "name": "Product 1",
      "price": "Rs. 500",
      "brand": "Brand Name",
      "category": {
        "usertype": { "usertype": "Men" },
        "category": "Shirts"
      }
    }
  ]
}
```

---

## 📚 **Folder Structure**
```
├── AutomationExercise.com.postman_collection.json   # Postman collection file
├── README.md                                       # Project documentation (this file)
└── Screenshots/                                    # (Optional) Add screenshots if needed
```

---

## 📊 **Test Results**

- ✅ **200 OK:** Successful API calls.
- 🚫 **405 Method Not Allowed:** For unsupported methods.
- ❗ **400 Bad Request:** Missing required parameters.
- ❌ **404 Not Found:** Invalid login credentials.

---



## 💡 **License**

This project is licensed under the MIT License.



⭐ **If you like this project, don't forget to give it a star!** ⭐

