# 📘 Database Naming Standards – MySQL

## 📅 Date: 20-06-2025
## 👩‍💻 Author: Divya Priya

---

## 🔤 General Naming Rules
- Only use: letters (A-Z, a-z), numbers (0-9), and underscores (_)
- Names must start with a letter
- Avoid using reserved keywords (e.g., `select`, `from`)
- Avoid spaces and special characters

## 🗃️ Database Name
- Use lowercase letters only
- Use underscores (_) instead of spaces
- Be short but meaningful
- ✅ Example: `hrms_portal`, `inventory_system`
- ⚠️ Limit: 64 characters

## 📋 Table Name
- Use lowercase with underscores
- Table names should be plural
- Prefix with module name if needed
- ✅ Example: `employee_records`, `product_reviews`
- ⚠️ Limit: 64 characters

## 📑 Column Name
- Use lowercase with underscores
- Use meaningful and consistent names
- For Boolean columns: `is_active`, `has_license`
- For foreign keys: `referenced_table_id`
- ✅ Example: `first_name`, `created_at`, `user_id`
- ⚠️ Limit: 64 characters

## 📌 Index and Constraint Names
- Use format: `idx_<table>_<column>`, `fk_<table>_<ref_table>`
- ✅ Example: `idx_employee_first_name`, `fk_order_user`
- ⚠️ Limit: 64 characters

## 📏 Character Limits Summary

| Item               | Limit (Characters) |
|--------------------|--------------------|
| Database Name      | 64                 |
| Table Name         | 64                 |
| Column Name        | 64                 |
| Alias Name         | 256                |
| Index Name         | 64                 |
| Constraint Name    | 64                 |

---

## ✅ Good Practices
- Use `snake_case` consistently
- Always use `created_at` and `updated_at` fields for timestamping
- Foreign keys should be indexed
- Avoid abbreviations unless well-known (e.g., `dob`, `ip_address`)

## ⚠️ Notes
- MySQL has a 64-character limit on identifiers (database, table, column, etc.)
- Avoid using camelCase or PascalCase
- Always double-check reserved keywords [MySQL reserved words list](https://dev.mysql.com/doc/refman/8.0/en/keywords.html)