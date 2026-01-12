
PROJECT: PRODUCT MANAGEMENT REST API (Task 2.A)
Hi there! Welcome to the Product Management API. This project 
was created as a learning milestone at Vistula University 
to demonstrate how to build a real-world backend using 
Spring Boot.

-----------------------------------------------------------
1. WHAT IS THIS?
-----------------------------------------------------------
Think of this as a digital "inventory list." It allows a 
user to create, view, update, and delete products through 
the internet. 

While most apps use a heavy database like PostgreSQL or 
MySQL, we have "humanized" this version for learning. 
Currently, it uses a HashMap (in-memory storage). It 
"pretends" to be a database to keep things simple while we 
focus on the API logic.

-----------------------------------------------------------
2. HOW THE PROJECT IS ORGANIZED
-----------------------------------------------------------
We use a "Layered Architecture," which is just a fancy way 
of saying everyone has a specific job:

* DOMAIN (Product.java): 
  The blueprint. It defines that every product must have 
  a name and a unique ID number.

* REPOSITORY (ProductRepository.java): 
  The storage room. It holds the HashMap and manages the 
  counter that gives every new product a unique ID.

* API LAYER: 
  The reception desk. This is where we handle the incoming 
  requests from the outside world (via ProductController).

* SERVICE & SUPPORT: 
  The "middle-men" that make sure data is formatted correctly 
  before it reaches the storage room.

-----------------------------------------------------------
3. HOW TO TALK TO THE API
-----------------------------------------------------------
You can use tools like Postman, Insomnia, or the built-in 
Swagger UI to test these commands:

[POST] Create a Product
URL: http://localhost:8080/api/v1/products
Body (JSON): { "name": "Tesla" }
Response: 201 Created (Success!)

[GET] View All Products
URL: http://localhost:8080/api/v1/products
This returns a list of everything you've added.

[GET] View One Product
URL: http://localhost:8080/api/v1/products/{id}
Replace {id} with the number of the product you want.

[DELETE] Remove a Product
URL: http://localhost:8080/api/v1/products/{id}
This removes the item from our temporary memory.

-----------------------------------------------------------
4. IMPORTANT NOTE ON DATA
-----------------------------------------------------------
Because we are using a HashMap, your data is "volatile." 
This means if you stop the application or restart your 
computer, the list will be wiped clean. In the next 
assignment, we will connect a permanent database to 
solve this!

![SS3 (3)](https://github.com/user-attachments/assets/f23a5ca7-1f6f-495d-b82e-4c5de6919186)
![SS2 (2)](https://github.com/user-attachments/assets/662b4125-5684-436a-a5cd-89b47b6994cc)
![SS1 (1)](https://github.com/user-attachments/assets/889454bf-9abf-4df2-858f-686efdb2626e)
![SS6 (6)](https://github.com/user-attachments/assets/f03e8972-2d98-43bd-a220-c3be7730a0f6)
![SS5 (5)](https://github.com/user-attachments/assets/e142dab7-7199-4917-baf2-5672f0f5ddca)
![SS4 (4)](https://github.com/user-attachments/assets/656099de-4dd8-4079-92c3-04034d1c4bca)

-----------------------------------------------------------
Vistula University - Akademia Finansow i Biznesu Vistula
Studia globalnych mozliwosci
===========================================================
