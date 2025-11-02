# Bug Reporting & Quality Analysis — TutorialsNinja & Herokuapp

## Project Overview

This project demonstrates a structured approach to **bug identification, documentation, and reporting** for two web applications used for software testing practice:

- [TutorialsNinja Demo Website](https://tutorialsninja.com/demo)
- [Herokuapp Testing Site](https://the-internet.herokuapp.com)

It was conducted as part of the **Software Testing & Quality Assurance** coursework in the **BS Software Engineering** program.  
The objective was to simulate a real-world QA workflow — from test exploration to defect documentation — using professional bug reporting standards.

---

## Project Objectives

The main goals of this project are to:

- Understand the **end-to-end bug reporting process**.  
- Identify **UI, Functional, and Content defects** through exploratory testing.  
- Document defects using a **structured and standardized Excel bug report format**.  
- Write **release notes** summarizing defects, fixes, and recommendations.  
- Demonstrate **professional QA documentation** suitable for team collaboration or client submission.

---

## Test Scope

| Parameter              | Details |
|------------------------|----------|
| **Application 1**      | TutorialsNinja Demo Store |
| **Application 2**      | The Internet (Herokuapp) |
| **Testing Type**       | Exploratory, Functional, UI, and Content Testing |
| **Environment**        | Web (Google Chrome, Edge) |
| **Platform**           | Windows 10 |
| **Testing Tools**      | Microsoft Excel (Bug Report), Manual Observation |

---

## 🛠️ Tools & Technologies Used

| Tool / Platform                  | Purpose |
|----------------------------------|----------|
| **Microsoft Excel**              | Used for structured bug reporting and release notes documentation |
| **Google Chrome DevTools**       | Used for inspecting broken elements, console errors, and UI issues |
| **TutorialsNinja Demo Website**  | E-commerce testing environment |
| **Herokuapp Testing Site**       | General-purpose test site for web scenarios |
| **VS Code (optional)**           | Used for documentation formatting |

---

## Bug Report Summary

### TutorialsNinja Defects

| Bug ID | Title | Severity | Priority | Type | Page / Area | Steps to Reproduce | Expected Result | Actual Result | Recommendation |
|--------|--------|-----------|-----------|------|---------------|--------------------|------------------|----------------|----------------|
| **TN001** | Stray text “123456789” in header | Minor | Low | UI | Homepage | Open Homepage → Observe top navigation | Header should display menu only | Extra text “123456789” appears | Remove placeholder or debug text |
| **TN002** | “Add to Cart” active for Out of Stock product | Major | High | Functional | Product Detail Page (MacBook) | Open an “Out of Stock” product → Click Add to Cart | Add to Cart should be disabled | Product still adds to cart | Disable button when stock = 0 |
| **TN003** | Price format displays “##” before amount | Minor | Low | UI | Product Detail Page | Open any product → Check price | Price should display cleanly | Price shows “## $602.00” | Fix price formatting template |
| **TN004** | Duplicate label fields on “Forgot Password” page | Minor | Low | UI | Forgot Password | Navigate to Forgot Password → Observe labels | Single Email label should appear | Duplicate labels “Your E-Mail Address” and “E-Mail Address” | Remove redundant label element |

---

### Herokuapp Defects

| Bug ID | Title | Severity | Priority | Type | Page / Area | Steps to Reproduce | Expected Result | Actual Result | Recommendation |
|--------|--------|-----------|-----------|------|---------------|--------------------|------------------|----------------|----------------|
| **HI001** | Broken images on “Broken Images” page | Major | High | Functional | `/broken_images` | Open page → Observe image thumbnails | All images load properly | Several images fail to load | Replace or fix broken image links |
| **HI002** | Login error message unclear for invalid user | Medium | Medium | UX / Functional | `/login` | Enter invalid credentials → Submit | Should show clear “Invalid username or password” | Error message unclear and inconsistent | Update message text and style |
| **HI003** | Checkbox state resets on refresh | Minor | Low | Functional | `/checkboxes` | Tick checkbox → Refresh page | Checkbox should retain selected state | State resets | Implement state persistence (session/local storage) |
| **HI004** | Typographical error on “Typos” page | Minor | Low | Content | `/typos` | Open page → Read paragraph | Text should be grammatically correct | Shows “won,t” instead of “won’t” | Correct typographical errors |

---

## Defect Summary Table

| Application | Total Defects | Major | Medium | Minor |
|--------------|----------------|---------|----------|---------|
| TutorialsNinja | 4 | 1 | 0 | 3 |
| Herokuapp | 4 | 1 | 1 | 2 |
| **Total** | **8** | **2** | **1** | **5** |

---

## Release Notes

| Section | Details |
|----------|----------|
| **Project Title** | Bug Reporting and QA Documentation for TutorialsNinja & Herokuapp |
| **Release Version** | v1.0 |
| **Prepared By** | Ayesha Ismail |
| **Date** | November 2025 |
| **Summary** | A total of 8 defects were logged across both testing sites. 2 Major, 1 Medium, and 5 Minor issues were identified related to UI, Functional, and Content areas. |
| **Fixed / Pending** | Pending — No developer fixes applied yet (report-only stage) |
| **Next Steps** | Review critical issues (TN002, HI001), assign for fixing, and conduct re-testing after patch. |
| **Notes** | Screenshots, detailed descriptions, and recommendations provided within Excel report. |

---

##  Folder Structure

Bug-Reporting-TutorialNinja-Herokuapp/
│
├── 📁 reports/
│ └── bug_reports_tutorialninja_herokuapp.xlsx # Complete bug report and release notes
│
├── 📄 README.md # Documentation file

