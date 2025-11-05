# Practice Software Testing API

## 🌐 Base URL
- https://api.practicesoftwaretesting.com

## 🔐 Authentication
- Uses **Bearer Token** for protected endpoints.
- Admin endpoints require **admin privileges**.
- Example login credentials:
  - **Admin:** admin@practicesoftwaretesting.com / welcome01  
  - **User:** customer@practicesoftwaretesting.com / welcome01

## 📦 Key Endpoints

### Users
- **Login:** `POST /users/login`  
- **Register:** `POST /users/register`  
- **Get Current User:** `GET /users/me`  

### Products
- **Get all products:** `GET /products`  
- **Get product by ID:** `GET /products/{product_id}`  
- **Create/Update/Delete product:** Admin only

### Orders
- **Get user orders:** `GET /orders`  
- **Create order:** `POST /orders`  
- **Update order status:** Admin only  

### Categories & Brands
- **Get all categories:** `GET /categories`  
- **Get all brands:** `GET /brands`  
- Admin can create/update/delete

## 📝 Notes
- Use **JSON** for requests and responses.
- Always include **Bearer token** for protected routes.
- All list endpoints support **pagination**: `?page=1&per_page=9`
- Sorting & filtering available for products: `?search=term&sort=price&order=asc`
