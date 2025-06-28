# Government TMS – SRS Evaluation

> Based on the specification by Osamah Yacoub and Ahmad Arrabi, finalized on December 31, 2002

---

## 1. Who created the final version?

The final Version 1.0 of the SRS was authored by:

- Osamah Yacoub
- Ahmad Arrabi

On December 31, 2002, they finalized:
- Functional and non-functional requirements
- Use cases
- Component business priorities

---

## 2. What is the intended use?

The SRS defines the specifications for a Training Management System (TMS) used in e-Government operations. Specifically, it is a web-baesd system "to acquire and track training and testing sessions for Government of Jordan (GoJ) employee"s 
The system is designed to:

- Track employee training and testing
- Manage registration and results
- Generate relevamt reports 
- Accept course feedback from the trainees 

It provides a structured framework for managing employee development activities within government agencies.

---

## 3. Who are the intended users?

The system is targeted at the following user roles:

- System Administrators
- PMU Administrators
- Training Provider (TP) Administrators
- Training Coordinator (TC)
- Government of Jordan (GoJ) Employees

---

## 4. What is the standard environment?

The TMS operates in a web-based environment (internet, intranet) with the following technical specifications:

- Browser: Microsoft Internet Explorer 5.0 or higher
- Languages: English and Arabic
- Display Resolution Optimally 800×600
- Environment: Requires a pre-established runtime, networking, hardware, and software setup

---

## 5. Functional Requirement Evaluation: `FR20.3 – Export to Excel`

> **Description**: “Export to Excel: Provide the ability to export report data to Microsoft Excel (for further analysis).”


- **Complete**  Partially. The requirement mentions exporting but lacks detail about which reports, fields, and filters are involved.
- **Accurate** Yes, the Excel export functionality is a valid and useful feature for a TMS. 
- **Unambiguous** No, it is vague. It does not specify the format (`.csv` or `.xlsx`), the data structure, or the exact behavior of the export feature.
- **Traceable** Yes, this requirement could be traced/linked to other relevant FR dimensions
-  **Testable**  Not testable as written. To become testable, it should include criteria like:
   - Excel file downloads correctly
   - File includes correct headers and fields
   - No data loss
   - Support for Arabic and English characters
   - Excel 2000+ compatibility |

---

## 6. Is there a requirement regarding data security?

Yes, the system includes security-related requirements such as SYS03, which defines:

- User role-based access control
-   Differentiated access rights based on administrative role
-   Implicit protection of sensitive data (e.g., test results)

But overall these are sparse and insufficient. 

---

## 7. Is there a requirement for software design?

Partially. There is no direct mention of design patterns, system architecture, or similar considerations. While not explicitly detailed in architectural terms, the SRS implies some design constraints through:
- Role-based permission structure
- Modular business logic aligned with user responsibilities


---

by Sarah Deckarm, 2025
