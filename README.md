# 🚀 User Management API Documentation

**Base URL:** `http://localhost:8080`

---

## 🛠️ Daftar Endpoint (Methods)

### 1. ➕ Tambah User Baru (POST)
**Endpoint:** `/api/users`  
**Fungsi:** Menambahkan data user baru ke database.

**Request Body (JSON):**
```json
{
  "name": "Fakhri",
  "age": "12"
}
```
Respon Sukses (201 Created):
```json
{
  "data": {
    "age": 12,
    "id": "4be0d21d-87cf-4922-8c25-2c635a091511",
    "name": "Fakhri"
  },
  "status": "success"
}
```

### 2. ➕ Melihat  User (GET)
**Endpoint:** `/api/users`  
**Fungsi:** Melihat data user baru.

**Respon Sukses (200):*

```json

{
  "data": [
    {
      "age": 11,
      "id": "237176e8-0f90-447f-a967-f3033fac8c6b",
      "name": "Asharfillah"
    },
    {
      "age": 9,
      "id": "3020ba75-ddb0-4144-a162-503b7fe754db",
      "name": "Farhat"
    }
  ],
  "status": "success"
}
```



### 3. ➕ Edit User  (PUT)
**Endpoint:** `http://localhost:8080/api/users/4be0d21d-87cf-4922-8c25-2c635a091511`  
**Fungsi:** Mengedit data user baru.

**Request Body (JSON):*

```json

{
  "name": "Fakhri",
  "age": "25"
}
```
Respon Sukses (200):
```json
{
  "data": {
    "age": 25,
    "id": "4be0d21d-87cf-4922-8c25-2c635a091511",
    "name": "Fakhri"
  },
  "status": "success"
}
```



### 4. ➕ Delete User  (DELETE)
**Endpoint:** `http://localhost:8080/api/users/0e467055-6bca-4fe4-9f18-70d74623e3d8`  
**Fungsi:** Menghapus data user.

**Request Body (JSON):*

```json
{
  "name": "Fakhri",
  "age": "25"
}
```
Respon Sukses (200):
```json
{
    "status": "success delete user with id 4be0d21d-87cf-4922-8c25-2c635a091511"
}
```
<img width="1918" height="967" alt="Cuplikan layar 2026-03-02 114011" src="https://github.com/user-attachments/assets/aa18ecab-f60b-4fde-81bc-899de522b91b" />

