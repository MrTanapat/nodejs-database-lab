# Testing the API with Postman
**1. Health Check**
```
GET http://localhost:3000/
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Students/Health%20Check.png" width="800" height="600">

**2. ดึงข้อมูลนักเรียนทั้งหมด**
```
GET http://localhost:3000/api/students
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Students/Get%20all%20Students.png" width="800" height="600">

**3. เพิ่มนักเรียนใหม่**
```
POST http://localhost:3000/api/students
Content-Type: application/json

{
    "firstName": "สมชาย",
    "lastName": "ใจดี", 
    "email": "somchai@email.com",
    "age": 20,
    "major": "Computer Science"
}
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Students/newStudents.png" width="800" height="600">

**4. ดึงข้อมูลนักเรียนตาม ID**
```
GET http://localhost:3000/api/students/1
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Students/GetFromID.png" width="800" height="600">

**5. อัพเดทข้อมูลนักเรียน**
```
PUT http://localhost:3000/api/students/1
Content-Type: application/json

{
    "firstName": "สมชาย",
    "lastName": "ใจดี Updated",
    "email": "somchai.updated@email.com", 
    "age": 21,
    "major": "Data Science"
}
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Students/UpdateStudentInfo.png" width="800" height="600">

**6. ลบนักเรียน**
```
DELETE http://localhost:3000/api/students/1
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Students/DeleteStudentsFromID.png" width="800" height="600">

#### 🟢 ทดสอบ Products API (MongoDB)

**1. ดึงข้อมูล products ทั้งหมด**
```
GET http://localhost:3000/api/products
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Products/GetAllProducts.png" width="800" height="600">

**2. เพิ่ม product ใหม่**
```
POST http://localhost:3000/api/products
Content-Type: application/json

{
    "name": "iPhone 15",
    "price": 35000,
    "category": "Electronics",
    "inStock": true,
    "quantity": 10
}
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Products/AddNewProduct.png" width="800" height="600">

**3. เพิ่ม product อีกตัว**
```
POST http://localhost:3000/api/products
Content-Type: application/json

{
    "name": "MacBook Pro",
    "price": 65000,
    "category": "Electronics",
    "inStock": true,
    "quantity": 5
}
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Products/AddNewProduct2.png" width="800" height="600">

**4. ดึงข้อมูล product ตาม ID**
```
GET http://localhost:3000/api/products/ObjectId_ที่ได้จาก_response
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Products/GetProdcutFromId.png" width="800" height="600">

**5. อัพเดท product**
```
PUT http://localhost:3000/api/products/ObjectId_ที่ได้จาก_response
Content-Type: application/json

{
    "name": "iPhone 15 Pro",
    "price": 42000,
    "quantity": 8
}
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Products/UpdateProductFromID.png" width="800" height="600">

**6. ลบ product**
```
DELETE http://localhost:3000/api/products/ObjectId_ที่ได้จาก_response
```
<img src="https://github.com/MrTanapat/nodejs-database-lab/blob/main/PreLab6Image/Products/DeleteProductFromId.png" width="800" height="600">

---
