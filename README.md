# eTax Library – Backend Engineering Case Study

A comprehensive legal and tax research platform developed under the “Ladhani Tax Guide” brand, built entirely from the ground up using a hybrid tech stack across web, desktop, mobile, and admin systems. Designed for cross-platform usage by Pakistan’s top tax advisory firms (including PwC, EY, KPMG, and FBR), the system handles secure access to over 100,000 tax documents, real-time updates, subscription billing, and licensing controls.

> 📌 This case study showcases the backend architecture, deployment automation, and system integrations performed across a multi-year development cycle.

---

## ⚙️ Tech Stack Overview

- **Languages:** C#, VB.NET, Python
- **Frameworks:** ASP.NET Core, .NET MAUI/Xamarin, Flask
- **Database:** SQL Server 2019+ (100,000+ documents, custom indexing)
- **Tools:** RedGate SQLCompare, PowerShell, InnoSetup, GitHub Actions, DevExpress
- **Deployment:** Windows Server 2022, IIS, self-hosted CI/CD and licensing
- **Other:** Licensing, SQL Server Express Automation, WebView, WinForms, RBAC

---

## 🔧 What I Built

### 💻 Web Application (ASP.NET + SQL Server)
- Built the **public-facing web application** with secure authentication, data search, and document delivery.
- User registration, password reset, license validation, and usage analytics via custom middleware.
- Optimized search engine for fast lookup across 100,000+ indexed legal/tax entries.

### 🌐 Website Platform (Flask + SQL)
- Developed the company’s **official web portal** using Flask for secure logins, account management, and billing.
- Integrated direct **bank payment systems** for user subscriptions and license activation.
- Performed backend billing workflows and asynchronous license provisioning.

### 🖥️ Desktop Application (WinForms / .NET Framework + SQL Server)
- Created a **desktop research suite** supporting offline caching and synced access to licensed document data.
- Integrated a custom **licensing engine** in VB.NET to prevent piracy.
- Delivered as a **click-to-install package** bundled with SQL Server Express and fonts via InnoSetup.

### 🔐 License Key Generator (VB.NET)
- Built a hardware-bound **keygen and license validation system** in VB.NET.
- Designed for limited-time and device-specific activation to ensure compliance.

### 🧠 Document Database (SQL Server)
- Engineered a SQL Server database to host **100,000+ tax and legal documents** with:
  - Custom schema optimized for full-text search and category tagging
  - Relationships for document types, legal references, authorship, and date-based retrieval
  - Versioning system to track content changes across years

### 🛠️ Database Management Suite (Admin App in .NET)
- Developed a standalone **admin desktop application** to manage and configure all SQL data.
- Features include content editing, version control, user metadata tagging, audit history, and full admin RBAC.
- Interfaces built with DevExpress for advanced control grids and UI flexibility.

### 🧾 Admin Panel (WinForms + SQL)
- Built a second .NET-based **admin interface** to manage end-user accounts, licenses, and payment history.
- Provided bulk user provisioning, usage logs, and billing reconciliation.

### 📱 Mobile Application (WebView in .NET MAUI + Xamarin)
- Created a **hybrid mobile app** for iOS and Android using WebView.
- Connected to the main Flask-based website and provided secure authentication + content previews.

### ⚙️ Installer Automation (InnoSetup + PowerShell)
- Wrote a complete **installer script** to bundle:
  - Desktop app binaries
  - SQL Server Express 2019
  - Required fonts
  - Configuration files
- One-click installation with silent mode and auto-start
- Future release planned on GitHub

### 🔄 Weekly Database Sync System
- Used **RedGate SQLCompare** and PowerShell to:
  - Compare production and master SQL Server databases
  - Generate weekly **delta scripts** automatically
  - Push secure update files to end-user desktop apps for seamless syncing

### 🖥️ Hosting & Infrastructure (Windows Server 2022)
- Purchased, set up, and secured a self-hosted **Windows Server 2022 VPS**
- Deployed IIS for web hosting, SQL Server for database backend, and CI jobs for automated deploys

## 📐 Architecture Overview

```
                [ Users ]
                    ↓
    ┌────────────────────────────────┐
    │  Desktop App (.NET / SQL)      │
    │  Web App (ASP.NET / Flask)     │
    └────────────────────────────────┘
                    ↓
            [ Backend APIs ]
   (ASP.NET Core + Flask + SQL Logic)
                    ↓
        [ SQL Server 2019 Database ]
   (100,000+ documents, RBAC, search)
                    ↓
    [ Admin Tools / Sync Engine / CI ]
```

## 🧪 Testing & Quality Assurance

- Unit testing with xUnit (desktop), PyTest (web), and manual QA cycles
- CI/CD pipelines for build + deployment (GitHub Actions + PowerShell)
- Audit logging and license validation checks on all user flows

---

## 📬 Contact & Credits

📧 [ladhanisahil@proton.me](mailto:ladhanisahil@proton.me)  
🔗 [github.com/sahilladhani](https://github.com/sahilladhani)  

> 💡 This case study reflects solo development and engineering leadership over a multi-phase product lifecycle. Project is live under the “Ladhani Tax Guide” brand.
