# Cloud-Based Hostel Complaint Management System using Zoho Creator (SaaS)

## 📌 Project Overview
This repository contains the complete implementation, database schemas, Deluge cloud workflows, and assignment deliverables for the **Cloud-Based Hostel Complaint Management System** developed on **Zoho Creator** (Software as a Service - SaaS).

---

## 📂 Repository Contents
- 📄 `Hostel_Complaint_Management_System_Assignment.docx`: Comprehensive Word Document formatted according to the official `COMMON COURSE ASSIGNMENT FORMAT`.
- 📁 `Output_images/`: Original application output screenshots.
- 📁 `deluge_scripts/`: Zoho Creator Deluge event automation scripts.

---

## 🛠️ Deluge Workflow Code (Zoho Creator)

```deluge
// On Success Workflow - Hostel Complaint Form
void complaint_on_submit()
{
    if(input.Status == null || input.Status == "")
    {
        input.Status = "Open";
    }
    if(input.Date_Submitted == null)
    {
        input.Date_Submitted = zoho.currentdate;
    }
    if(input.Priority == "High")
    {
        info "ALERT: High priority complaint submitted for Room: " + input.Hostel_Room_Number;
    }
}
```

---

## 🎓 Academic Details
- **Department**: Computer Science and BioScience Engineering
- **Programme**: B.Tech
- **Course**: Cloud Computing and Big Data Analytics
- **Faculty**: Dr.K.Santhiya Lakshmi
- **Batch**: 2023-2027
