# 📘 Database Naming Standards – MySQL

## 📅 Date: 20-06-2025  
## 👩‍💻 Author: Divya Priya

---

### 1️⃣ Database Names
Use lowercase with underscores: `hospital_db`, `finance_system`

### 2️⃣ Table Names
Use plural + snake_case: `patients`, `medical_records`

### 3️⃣ Column Names
Use snake_case and be descriptive: `created_at`, `doctor_id`

### 4️⃣ Datatypes

| Data Type    | Use Case              |
|--------------|------------------------|
| INT          | Auto-increment IDs     |
| VARCHAR(255) | Names, emails, etc     |
| DATETIME     | Created/updated times  |
| TEXT         | Longer descriptions    |

### ⚠️ Notes:
- MySQL limit: 64 characters for identifiers
- Use `_id` for foreign keys
- Avoid camelCase and reserved keywords
