# AS/400 MODULES REFERENCE
## MOB Modules Reference

---

## 📋 COMPLETE MODULES LIST

| Module | Name | Purpose | Category |
|--------|------|---------|----------|
| **MOB201** | Batch Suspense File Booking | Batch processing of suspended operations | Batch Processing |
| **MOB206** | Base Module 206 | Basic functional module | Base Module |
| **MOB206OB** | Object Binary Module 206 | Object binary module | Data Communication |
| **MOB207** | Base Module 207 | Basic functional module | Base Module |
| **MOB207OB** | Object Binary Module 207 | Object binary module | Data Communication |
| **MOB208** | Base Module 208 | Basic functional module | Base Module |
| **MOB208DCC** | Data Communication | Data communication module | Data Communication |
| **MOB209** | Base Module 209 | Basic functional module | Base Module |
| **MOB209ENC** | Encoder Module | Encoding module | Data Communication |
| **MOB210** | Base Module 210 | Basic functional module | Base Module |
| **MOB216** | Base Module 216 | Basic functional module | Base Module |
| **MOB217** | Base Module 217 | Basic functional module | Base Module |
| **MOB258** | Billing Sequence Processing | Billing sequence processing | Batch Processing |
| **MOB259** | Base Module 259 | Basic functional module | Base Module |
| **MOB259PRE** | Pre-compile Module 259 | Pre-compilation | Utilities |
| **MOB265** | Insurance Billing "Upload" | Billing data upload | Insurance Billing |
| **MOB266** | Insurance Billing "Allocate" | Billing allocation | Insurance Billing |
| **MOB267** | Insurance Billing | Main billing module | Insurance Billing |
| **MOB268** | Base Module 268 | Basic functional module | Base Module |
| **MOB269** | Base Module 269 | Basic functional module | Base Module |
| **MOB269P** | Phase Module 269 | Phase claims processing | Insurance Claims |
| **MOB269P1** | Phase Module 269-1 | Phase claims processing (stage 1) | Insurance Claims |
| **MOB269P2** | Phase Module 269-2 | Phase claims processing (stage 2) | Insurance Claims |
| **MOB269X** | Load Insurance Claims | Claims loading | Insurance Claims |
| **MOB269XP** | Detail Claims to Excel | Claims detail to Excel | Insurance Claims |
| **MOB269XP2** | Detail Claims to Excel v2 | Enhanced claims detail | Insurance Claims |
| **MOB290** | Debt Protection Driver | Main debt protection program | Debt Protection |
| **MOB291** | Debt Protection Date Delete | Date range deletion | Debt Protection |
| **MOB292** | Debt Protection Lvl #2 Filter | Level 2 filter | Debt Protection |
| **MOB293** | Debt Protection Lvl #3 Filter | Level 3 filter | Debt Protection |
| **MOB294** | Debt Protection Lvl #3 Filter v2 | Level 3 filter (version 2) | Debt Protection |
| **MOB295** | Debt Protection Write CMPALCP | Write CMPALCP records | Debt Protection |

---

## 🏦 INSURANCE BILLING (3 modules)

### MOB265 - Insurance Billing "Upload"
**What it does:** Uploads billing data to the system  
**When used:** When receiving new insurance data  
**Input data:** Files with policy and premium data  
**Output data:** Validated data for processing  

### MOB266 - Insurance Billing "Allocate"
**What it does:** Allocates billing to clients and products  
**When used:** When calculating premiums and commissions  
**Input data:** Policy and rate data  
**Output data:** Allocated amounts by accounts  

### MOB267 - Insurance Billing
**What it does:** Main billing processing module  
**When used:** Daily for creating invoices  
**Input data:** Allocated billing data  
**Output data:** Client invoices and reports  

---

## 📋 CLAIMS PROCESSING (6 modules)

### MOB269X - Load Insurance Claims
**What it does:** Loads claims into the system  
**When used:** When new insurance cases arrive  
**Input data:** Insurance claim applications  
**Output data:** Registered claims  

### MOB269XP - Detail Claims to Excel
**What it does:** Creates detailed claims reports  
**When used:** For analysis and reporting  
**Input data:** Claims data  
**Output data:** Excel files with reports  

### MOB269XP2 - Detail Claims to Excel v2
**What it does:** Enhanced claims export version  
**When used:** For extended analytics  
**Input data:** Claims data  
**Output data:** Extended Excel reports  

### MOB269P - Phase Module 269
**What it does:** Phase-based claims processing  
**When used:** For complex cases  
**Input data:** Claims for phased processing  
**Output data:** Stage results  

### MOB269P1 - Phase Module 269-1
**What it does:** First stage of claims processing  
**When used:** Initial investigation phase  
**Input data:** New claims  
**Output data:** Initial assessment  

### MOB269P2 - Phase Module 269-2
**What it does:** Second stage of claims processing  
**When used:** Final investigation phase  
**Input data:** First stage results  
**Output data:** Final decision  

---

## 🛡️ DEBT PROTECTION (6 modules)

### MOB290 - Debt Protection Driver
**What it does:** Coordinates debt protection process  
**When used:** Daily for monitoring  
**Input data:** Debt data  
**Output data:** Collection action plan  

### MOB291 - Debt Protection Date Delete
**What it does:** Removes outdated records  
**When used:** Weekly for cleanup  
**Input data:** Historical data  
**Output data:** Cleaned database  

### MOB292 - Debt Protection Lvl #2 Filter
**What it does:** Filters clients by risk criteria  
**When used:** When analyzing debt  
**Input data:** Client and payment data  
**Output data:** Filtered client groups  

### MOB293 - Debt Protection Lvl #3 Filter
**What it does:** Detailed filtering by financial indicators  
**When used:** For deep risk analysis  
**Input data:** Client financial data  
**Output data:** High-risk clients  

### MOB294 - Debt Protection Lvl #3 Filter v2
**What it does:** Enhanced filtering with machine learning  
**When used:** For complex risk analysis  
**Input data:** Extended financial data  
**Output data:** Accurate risk assessment  

### MOB295 - Debt Protection Write CMPALCP
**What it does:** Writes debt protection measures  
**When used:** When making collection decisions  
**Input data:** Filtering results  
**Output data:** Collection action records  

---

## ⚙️ BATCH PROCESSING (2 modules)

### MOB201 - Batch Suspense File Booking
**What it does:** Processes large volumes of data  
**When used:** Nightly for batch processing  
**Input data:** Arrays of insurance data  
**Output data:** Processed records  

### MOB258 - Billing Sequence Processing
**What it does:** Manages billing operation sequence  
**When used:** When creating invoices  
**Input data:** Billing operations  
**Output data:** Ordered operations  

---

## 🔗 DATA COMMUNICATION (4 modules)

### MOB206OB - Object Binary Module 1
**What it does:** Processes binary data  
**When used:** When transferring files  
**Input data:** Binary files  
**Output data:** Processed objects  

### MOB207OB - Object Binary Module 2
**What it does:** Extended binary data processing  
**When used:** For complex operations  
**Input data:** Complex binary data  
**Output data:** Optimized objects  

### MOB208DCC - Data Communication
**What it does:** Exchanges data with external systems  
**When used:** Constantly for synchronization  
**Input data:** Data from external systems  
**Output data:** Data for external systems  

### MOB209ENC - Encoder Module
**What it does:** Encrypts and encodes data  
**When used:** When transferring sensitive data  
**Input data:** Open data  
**Output data:** Encrypted data  

---

## 🔧 UTILITIES (1 module)

### MOB259PRE - Pre-compile Module
**What it does:** Pre-compiles modules  
**When used:** During development and testing  
**Input data:** Source code  
**Output data:** Code prepared for compilation  

---

## 📊 MODULE STATISTICS

### By Category
- **Base Modules:** 21 (MOB201-217, MOB258-259, MOB268-269)
- **Insurance Billing:** 3 (MOB265-267)
- **Claims Processing:** 6 (MOB269X, MOB269XP, MOB269XP2, MOB269P, MOB269P1, MOB269P2)
- **Debt Protection:** 6 (MOB290-295)
- **Batch Processing:** 2 (MOB201, MOB258)
- **Data Communication:** 4 (MOB206OB, MOB207OB, MOB208DCC, MOB209ENC)
- **Utilities:** 1 (MOB259PRE)

### By Complexity
- **High complexity (>500 records):** 5 modules
- **Medium complexity (200-500 records):** 15 modules
- **Low complexity (<200 records):** 12 modules

---

## ⚠️ MIGRATION PLANS

### Modules to be replaced with C# Window Service
- **MOB290-295** - all Debt Protection modules
- **Reason:** AS/400 marked as "Decommissioned long ago"
- **Replacement:** C# Window Service with functions:
  - FTP monitoring
  - Certificate verification
  - Value verification
  - Value matching

### Modules that remain
- **MOB201-269** - all other modules
- **Status:** Continue to run on AS/400

---

**Creation Date:** September 30, 2024  
**Version:** 1.0  
**Status:** Current

## 🏷️ TAGS

`AS/400` `MOB Modules` `Insurance System` `Claims Processing` `Billing Management` `Debt Protection` `Module Reference` `Business Functions`