# Mini Account Management System

A secure and structured ASP.NET Core Razor Pages project built for managing Chart of Accounts and Vouchers with role-based access. Developed as an assignment for "Qtec Solution Limited".

----
## Live Modules

### 1. Voucher Management
- Create, View, Edit, Delete vouchers
- Uses `sp_SaveVoucher` stored procedure with Table-Valued Parameters

### 2. Chart of Accounts
- Add Parent/Child accounts
- Uses `sp_ManageChartOfAccounts` stored procedure

---

## Role-Based Access

### Admin
- Full Access to all modules

### Accountant
- ✅ Create/Edit Vouchers
- ✅ Manage Chart of Accounts
- ❌ Cannot manage roles or users

### Viewer(Read-only)
| Module                | Access Status      | URL                            |
|-----------------------|--------------------|---------------------------------|
| 🏠 **Home**            | ✅ View             | `/` or `/Index`                |
| 📄 **Accounts List**   | ✅ View             | `/Accounts/Index`              |
| 🧾 **Voucher List**    | ✅ View             | `/Vouchers/Index`              |
| 📄 **Voucher Details** | ✅ View             | `/Vouchers/Details?id={id}`    |
| ✍️ **Create Voucher**   | ❌ Not Allowed      | `/Vouchers/Create`             |
| ➕ **Add Account**      | ❌ Not Allowed      | `/Accounts/Create`             |

---

## Technologies Used
- ASP.NET Core Razor Pages (.NET 7)
- SQL Server (Stored Procedures)
- ASP.NET Core Identity
- Role-based authorization
- Bootstrap 5 UI
- Azure data studio

---

## onus Feature (Optional)
- ✅ Export Vouchers to Excel (.xlsx)
  - Click `📥 Export to Excel` button on the Vouchers page

---

##  How to Run
1. Clone the repo
2. Update `appsettings.json` with your SQL connection string
3. Run the database script (Tables + Stored Procedures)
4. Run project using `dotnet run`

OR 

1. Download the project
2. Open Project in visual studio
3. Run project using `dotnet run`

---

## 📸 Screenshots

### 🏠 Home Page
![Home](screenshots/home.png)

### 📄 Chart of Accounts
![Accounts](screenshots/accounts.png)

### 🧾 Voucher Entry
![Voucher](screenshots/voucher.png)

### 🔐 Role Access Control
![Roles](screenshots/roles.png)

### 📤 Export to Excel
![Export](screenshots/export.png)

---


### Developed  by Foysal

For any issues, feel free to raise a GitHub issue or email with your feedback.

