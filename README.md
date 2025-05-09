# Driver License Management System 🚗🛂

A complete desktop application for managing driver license processes with user roles, logging, data security, and a clean architecture using C# and SQL Server.

![Driver License Preview](https://images.openai.com/thumbnails/646fdb7e1072c78a21e0ab3fa1621636.jpeg)

---

## 🔧 Features

* **User Events & DataBack Delegates**
* **Extension Methods** to enhance code readability and reuse
* **Error Handling**: `try-catch` blocks with error logging to Windows Registry
* **User-Friendly Messages** for better UX
* **Filtering** data dynamically
* **Complete CRUD Operations** on all entities
* **Clean, Maintainable & Readable Code**
* **Advanced Validations** (Email, Egyptian phone numbers, etc.)
* **User Roles & Permissions** (`Admin`, `Editor`, `Viewer`)
* **Detailed Operation Logs** (login, create, edit, delete)
* **File Handling** (store images, export reports)
* **Sensitive Data Security** (passwords hidden & hashed)
* **Database Layer**: Stored Procedures, Views, Triggers
* **3-Tier Architecture** with a dedicated `DBManager` for clean data access
* **2 Modes (AddNew, Update)** per screen for reusability with unified `Save()` function
* **Extensive Use of User Controls** for modular and reusable UI components
* **Quick Navigation** with links between related screens
* **Lambda Expressions** for cleaner and more efficient code

---

## 📚 Application Workflow

1. **Employee Login**
   Employees log in with validated credentials based on their permission level.

2. **New Driver Registration**
   New driver information is entered, and a local license file is created.

3. **Testing Phase**

   * Drivers go through three mandatory tests:
     `Theory`, `Written`, and `Driving`.
   * All tests must be passed to issue a license.

4. **License Issuance & Renewal**

   * Once passed, a license is issued.
   * The driver can later apply for renewal, replacement (lost/damaged), or pay fines for violations.
   * Drivers may apply for multiple local licenses (for different vehicle categories).
   * After obtaining a local license, drivers can apply for an international license.

5. **Driver Record**

   * Once a license is issued for the first time, the driver is permanently recorded in the system.

---

## User Roles & Permissions implemented using efficient byte flags with bitwise & operations for screen-level access control (Admin, Editor, Viewer)



| Role   | Permissions                                                              |
| ------ | ------------------------------------------------------------------------ |
| Admin  | Full access (except adding/deleting license files or test types)         |
| Editor | Manage driver records, view reports, but can't edit employee/system data |
| Viewer | Read-only access                                                         |

---

## 📊 Reporting

* Admin users can view detailed logs:

  * User operations (create, edit, delete)
  * Registration dates and activity timestamps

---

## 📁 Architecture

* **UI Layer**: Windows Forms
* **Business Logic Layer**
* **Data Access Layer**
* **DBManager** for central data operations
* SQL Server for backend with use of:

  * Stored Procedures
  * Views
  * Triggers

---

## 🛠️ Development Environment

* Visual Studio Community 2022
* C# WinForms
* Libraries: `System.IO`, `Resources`, Image Processing, Text File Reporting

---

## 👥 Default Users

| Role   | Username | Password |
| ------ | -------- | -------- |
| Admin  | User1    | 1111     |
| Editor | User2    | 2222     |
| Viewer | User3    | 3333     |

To see all of my Projects Presentation , Please Visit My Telegram Channel :
https://t.me/ahmedelhwwary3

