# BRD - BUSINESS REQUIREMENTS DOCUMENT
## AS/400 Insurance Claims & Billing System

---

## 📋 EXECUTIVE SUMMARY

**System Name:** AS/400 Insurance Claims & Billing System  
**System Type:** Insurance policy and claims processing system  
**Platform:** IBM i (AS/400)  
**Programming Language:** IBM ILE RPG  
**Development Period:** September-October 2013  
**Status:** In production (migration to C# planned)  

---

## 🎯 BUSINESS OBJECTIVES

### Main Business Goals
- **Insurance Process Automation** - policy and claims processing
- **Billing Management** - invoice generation and payment management
- **Debt Protection** - preventing financial losses
- **Reporting and Analytics** - providing data for decision making

### Key Performance Indicators (KPI)
- **Claims processing time:** < 24 hours
- **Billing accuracy:** > 99.5%
- **System availability:** > 99.9%
- **Response time:** < 3 seconds

---

## 🏢 BUSINESS CONTEXT

### Insurance Industry
The MOB system is designed to automate key insurance company processes:

1. **Policy Management** - creating, modifying, renewing insurance policies
2. **Claims Processing** - registering, processing and settling insurance cases
3. **Billing** - invoice generation, payment management
4. **Debt Protection** - preventing financial losses from unpaid premiums

### System Users
- **Insurance Agents** - working with policies and clients
- **Claims Specialists** - processing insurance cases
- **Financial Analysts** - billing and reporting
- **System Administrators** - technical support

---

## 📊 BUSINESS PROCESSES

### 1. 🏦 INSURANCE POLICY MANAGEMENT

#### 1.1 Policy Creation
**Description:** Process of creating a new insurance policy

**Participants:**
- Insurance agent
- MOB system
- Policy database

**Process Steps:**
1. **Client Registration** - client data entry
2. **Insurance Type Selection** - determining insurance product type
3. **Premium Calculation** - determining insurance premium amount
4. **Policy Creation** - generating insurance policy
5. **Policy Activation** - putting policy into effect

**AS/400 Modules (MOB):**
- MOB201 - Batch Suspense File Booking
- MOB258 - Billing Sequence Processing

**Result:** Activated insurance policy

#### 1.2 Policy Modification
**Description:** Process of making changes to existing policy

**Process Steps:**
1. **Policy Search** - policy identification
2. **Change Validation** - checking change feasibility
3. **Adjustment Calculation** - premium recalculation
4. **Policy Update** - implementing changes
5. **Client Notification** - informing about changes

### 2. 📋 CLAIMS PROCESSING

#### 2.1 Claims Registration
**Description:** Process of registering new insurance case

**Participants:**
- Client/Claimant
- Claims specialist
- MOB system

**Process Steps:**
1. **Claim Receipt** - registering insurance claim
2. **Initial Assessment** - determining case type and complexity
3. **Specialist Assignment** - assigning claims specialist
4. **Document Collection** - requesting necessary documents
5. **Case Creation** - system registration

**AS/400 Modules (MOB):**
- MOB269X - Load Insurance Claims
- MOB269XP - Detail Claims to Excel
- MOB269XP2 - Detail Claims to Excel v2

**Result:** Registered insurance claim

#### 2.2 Claims Processing
**Description:** Process of investigating and settling claims

**Process Steps:**
1. **Investigation** - gathering information about insurance case
2. **Damage Assessment** - determining damage amount
3. **Coverage Verification** - analyzing policy terms
4. **Decision Making** - deciding on payment or denial
5. **Settlement** - payment or case closure

**AS/400 Modules (MOB):**
- MOB269P - Phase Module 269
- MOB269P1 - Phase Module 269-1
- MOB269P2 - Phase Module 269-2

### 3. 💰 BILLING MANAGEMENT

#### 3.1 Invoice Generation
**Description:** Process of creating and sending invoices

**Process Steps:**
1. **Premium Calculation** - determining payment amount
2. **Invoice Creation** - generating invoice
3. **Invoice Delivery** - sending to client
4. **Payment Monitoring** - tracking payments
5. **Payment Processing** - crediting payments

**AS/400 Modules (MOB):**
- MOB265 - Insurance Billing "Upload"
- MOB266 - Insurance Billing "Allocate"
- MOB267 - Insurance Billing

#### 3.2 Payment Management
**Description:** Process of managing client payments

**Process Steps:**
1. **Payment Receipt** - registering incoming payment
2. **Identification** - linking to specific invoice
3. **Validation** - checking payment correctness
4. **Crediting** - updating client balance
5. **Confirmation** - payment confirmation notification

### 4. 🛡️ DEBT PROTECTION

#### 4.1 Debt Monitoring
**Description:** Process of monitoring client debt

**Process Steps:**
1. **Debt Identification** - finding unpaid invoices
2. **Risk Analysis** - assessing collection probability
3. **Classification** - grouping by debt types
4. **Action Planning** - choosing collection strategy
5. **Result Monitoring** - tracking effectiveness

**AS/400 Modules (MOB):**
- MOB290 - Debt Protection Driver
- MOB291 - Debt Protection Date Delete
- MOB292 - Debt Protection Lvl #2 Filter
- MOB293 - Debt Protection Lvl #3 Filter
- MOB294 - Debt Protection Lvl #3 Filter v2
- MOB295 - Debt Protection Write CMPALCP

#### 4.2 Debt Collection
**Description:** Process of collecting outstanding debts

**Process Steps:**
1. **Reminders** - sending debt notifications
2. **Escalation** - transferring to collection agency
3. **Legal Actions** - filing court claims
4. **Collection** - forced debt recovery
5. **Closure** - writing off bad debt

---

## 🔄 INTEGRATION POINTS

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

## 📈 REPORTING & ANALYTICS

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

## ⚠️ NON-FUNCTIONAL REQUIREMENTS

### Performance Requirements
- **Response Time:** < 3 seconds for standard operations
- **Throughput:** 1000+ transactions per hour
- **Availability:** 99.9% uptime
- **Scalability:** Support for 10,000+ policies

### Security Requirements
- **Data Encryption:** All sensitive data encrypted
- **Access Control:** Role-based access control
- **Audit Trail:** Complete audit log
- **Backup:** Daily automated backups

### Compliance Requirements
- **Insurance Regulations:** Compliance with insurance laws
- **Data Protection:** GDPR compliance
- **Financial Reporting:** SOX compliance
- **Audit Requirements:** Internal and external audits

---

## 🎯 SUCCESS CRITERIA

### Business Success
- **Process Efficiency:** 50% reduction in processing time
- **Cost Reduction:** 30% reduction in operational costs
- **Customer Satisfaction:** > 95% customer satisfaction
- **Revenue Growth:** 20% increase in revenue

### Technical Success
- **System Stability:** < 1% error rate
- **Performance:** Meeting all performance requirements
- **Integration:** Successful integration with all systems
- **Migration:** Successful migration to C# for Debt Protection

---

## 👥 STAKEHOLDERS

### Primary Stakeholders
- **Insurance Company Management** - business owners
- **IT Department** - technical implementation
- **Insurance Agents** - end users
- **Claims Specialists** - end users

### Secondary Stakeholders
- **Clients** - policyholders
- **Regulatory Bodies** - compliance requirements
- **External Vendors** - system integration
- **Auditors** - system validation

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

### Migration Timeline
- **Phase 1:** Analysis and design (Q1 2025)
- **Phase 2:** Development and testing (Q2-Q3 2025)
- **Phase 3:** Deployment and cutover (Q4 2025)

---

**Document Creation Date:** September 30, 2024  
**Version:** 1.0  
**Status:** Current  
**Next Review:** December 30, 2024

## 🏷️ TAGS

`BRD` `Business Requirements` `AS/400` `Insurance System` `Claims Processing` `Billing Management` `Debt Protection` `Business Processes` `Stakeholders` `Success Criteria`