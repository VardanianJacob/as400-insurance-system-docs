# AS/400 SYSTEM BUSINESS DOCUMENTATION
## Insurance Claims & Billing System

---

## 📋 SYSTEM OVERVIEW

**System Name:** AS/400  
**Purpose:** Insurance policy and claims processing  
**Number of Modules:** 32 MOB modules  
**Status:** In production (migration to C# planned)  

---

## 🏢 BUSINESS PROCESSES

### 1. INSURANCE POLICY MANAGEMENT

#### Policy Creation
1. **Client Registration** - client data entry
2. **Insurance Type Selection** - determining insurance product type
3. **Premium Calculation** - determining insurance premium amount
4. **Policy Creation** - generating insurance policy
5. **Policy Activation** - putting policy into effect

#### Policy Modification
1. **Policy Search** - policy identification
2. **Change Validation** - checking change feasibility
3. **Adjustment Calculation** - premium recalculation
4. **Policy Update** - implementing changes
5. **Client Notification** - informing about changes

### 2. INSURANCE CLAIMS PROCESSING

#### Claims Registration
1. **Claim Receipt** - registering insurance claim
2. **Initial Assessment** - determining case type and complexity
3. **Specialist Assignment** - assigning claims specialist
4. **Document Collection** - requesting necessary documents
5. **Case Creation** - system registration

#### Claims Processing
1. **Investigation** - gathering information about insurance case
2. **Damage Assessment** - determining damage amount
3. **Coverage Verification** - analyzing policy terms
4. **Decision Making** - deciding on payment or denial
5. **Settlement** - payment or case closure

### 3. BILLING AND PAYMENTS

#### Invoice Generation
1. **Premium Calculation** - determining payment amount
2. **Invoice Creation** - generating invoice
3. **Invoice Delivery** - sending to client
4. **Payment Monitoring** - tracking payments
5. **Payment Processing** - crediting payments

#### Payment Management
1. **Payment Receipt** - registering incoming payment
2. **Identification** - linking to specific invoice
3. **Validation** - checking payment correctness
4. **Crediting** - updating client balance
5. **Confirmation** - payment confirmation notification

### 4. DEBT PROTECTION

#### Debt Monitoring
1. **Debt Identification** - finding unpaid invoices
2. **Risk Analysis** - assessing collection probability
3. **Classification** - grouping by debt types
4. **Action Planning** - choosing collection strategy
5. **Result Monitoring** - tracking effectiveness

#### Debt Collection
1. **Reminders** - sending debt notifications
2. **Escalation** - transferring to collection agency
3. **Legal Actions** - filing court claims
4. **Collection** - forced debt recovery
5. **Closure** - writing off bad debt

---

## 📊 MOB MODULES DESCRIPTION

### 1. INSURANCE BILLING

#### MOB265 - Insurance Billing "Upload"
**Purpose:** Uploading billing data to the system  
**Functions:**
- Loading insurance data from external sources
- Validating uploaded data
- Converting data formats
- Initializing billing process

#### MOB266 - Insurance Billing "Allocate"
**Purpose:** Allocating billing to clients  
**Functions:**
- Distributing insurance premiums across policies
- Calculating agent commissions
- Allocating costs by products
- Creating detailed billing records

#### MOB267 - Insurance Billing
**Purpose:** Main billing processing module  
**Functions:**
- Creating client invoices
- Processing payments
- Managing receivables
- Generating billing reports

### 2. CLAIMS PROCESSING

#### MOB269X - Load Insurance Claims
**Purpose:** Loading claims into the system  
**Functions:**
- Importing insurance case data
- Validating claims information
- Creating claims records
- Assigning claims specialists

#### MOB269XP - Detail Insurance Claims to Excel
**Purpose:** Detailed claims with Excel export  
**Functions:**
- Creating detailed claims reports
- Exporting data to Excel for analysis
- Filtering claims by various criteria
- Generating statistical reports

#### MOB269XP2 - Detail Insurance Claims to Excel (version 2)
**Purpose:** Enhanced claims export version  
**Functions:**
- Extended export functionality
- Additional filters and groupings
- Improved report formatting
- External system integration

### 3. DEBT PROTECTION

#### MOB290 - Debt Protection Allocation Driver Program
**Purpose:** Main debt protection allocation program  
**Functions:**
- Coordinating debt protection process
- Managing processing queue
- Monitoring operation status
- Logging all operations

#### MOB291 - Debt Protection Allocation Date Range Delete
**Purpose:** Deleting records by date range  
**Functions:**
- Removing outdated records
- Cleaning temporary data
- Archiving historical data
- Performance optimization

#### MOB292 - Debt Protection - Lvl #2 Filter
**Purpose:** Level 2 data filtering  
**Functions:**
- Filtering clients by risk criteria
- Grouping debt by types
- Applying business filtering rules
- Preparing data for further processing

#### MOB293 - Debt Protection - Lvl #3 Filter (FEEDTLL1)
**Purpose:** Level 3 data filtering  
**Functions:**
- Detailed filtering by financial indicators
- Client solvency analysis
- Applying complex risk assessment algorithms
- External data source integration

#### MOB294 - Debt Protection - Lvl #3 Filter (FEEDTLL1) v2
**Purpose:** Enhanced level 3 filtering version  
**Functions:**
- Extended filtering algorithms
- Machine learning for risk assessment
- Adaptive threshold values
- Improved performance

#### MOB295 - Debt Protection - Write CMPALCP Records
**Purpose:** Writing CMPALCP records  
**Functions:**
- Creating debt protection records
- Updating client status
- Generating notifications and reports
- Collection agency integration

### 4. BATCH PROCESSING

#### MOB201 - Batch Suspense File Booking
**Purpose:** Batch processing of suspended operations  
**Functions:**
- Processing large volumes of insurance data
- Managing job queue
- Monitoring processing progress
- Error and exception handling

#### MOB258 - Billing Sequence Processing
**Purpose:** Billing sequence processing  
**Functions:**
- Managing billing operation sequence
- Process synchronization
- Data integrity control
- Ensuring correct processing order

### 5. DATA COMMUNICATION

#### MOB206OB - Object Binary Module 1
**Purpose:** Object binary module  
**Functions:**
- Processing binary data
- Object serialization/deserialization
- Data transfer optimization
- Cache management

#### MOB207OB - Object Binary Module 2
**Purpose:** Object binary module (version 2)  
**Functions:**
- Extended binary data processing
- New format support
- Improved performance
- Additional security features

#### MOB208DCC - Data Communication
**Purpose:** Data communication module  
**Functions:**
- Data exchange with external systems
- FTP connection management
- Data synchronization
- Transfer protocol handling

#### MOB209ENC - Encoder Module
**Purpose:** Encoding module  
**Functions:**
- Encrypting sensitive data
- Information encoding/decoding
- Encryption key management
- Data security assurance

---

## 🔄 INTEGRATIONS

### External Systems
- **Four Point (Java/Oracle)** - main system
- **FTP Server** - file exchange
- **apsPlateau Database** - corporate database
- **BreakDown Values** - reference data

### Data Flows
1. **Four Point** → **FTP Server** → **AS/400** (certificate loading)
2. **AS/400** → **FTP Server** → **Four Point** (processing results)
3. **BreakDown Values** → **AS/400** (reference data)
4. **apsPlateau** → **AS/400** (client data)

---

## 📈 REPORTING

### Operational Reports
- **Policy Report** - insurance policy statistics
- **Claims Report** - insurance case analysis
- **Billing Report** - financial indicators
- **Debt Report** - receivables analysis

### Analytical Reports
- **Product Trends** - insurance product popularity analysis
- **Geographic Analysis** - regional distribution
- **Client Analysis** - client base segmentation
- **Forecasting** - claims and revenue predictions

---

## ⚠️ MIGRATION PLANS

### Current Status
- **AS/400 marked as "Decommissioned long ago"**
- **Planned replacement of Debt Protection modules (MOB290-295) with C# Window Service**

### C# Window Service Functions
- **FTP Monitoring** - tracking certificate files
- **Certificate Verification** (Cert is good)
- **Value Verification** (Values are good)
- **Value Matching** (Values match)

---

**Creation Date:** September 30, 2024  
**Version:** 1.0  
**Status:** Current

## 🏷️ TAGS

`AS/400` `Insurance System` `Claims Processing` `Billing Management` `Debt Protection` `MOB Modules` `Business Processes` `Policy Management` `Business Documentation`