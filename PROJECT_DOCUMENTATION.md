# AS/400 SYSTEM DOCUMENTATION (Insurance Claims & Billing System)

## SYSTEM OVERVIEW

**System Name:** AS/400 (Insurance Claims & Billing System)  
**System Type:** IBM i application on IBM ILE RPG for insurance policy and claims processing  
**Compiler Version:** 5722WDS V5R4M0  
**Development Period:** September-October 2013  
**Total MOB Modules:** 32  
**Functionality:** Insurance policy management, claims processing, billing, and debt protection  

## SYSTEM ARCHITECTURE

### MOB Modules Structure

The AS/400 system consists of 32 MOB modules organized by functional purpose:

#### 1. Base Modules (21 modules)
- **MOB201-MOB217**: Core functional modules
- **MOB258-MOB295**: Extended system modules

#### 2. Specialized Modules (11 modules)

**Pre-compile modules:**
- MOB259PRE - Pre-compilation

**Object Binary modules:**
- MOB206OB - Object binary module 206
- MOB207OB - Object binary module 207

**Communication modules:**
- MOB208DCC - Data communication module

**Encoder modules:**
- MOB209ENC - Encoding module

**Extended modules:**
- MOB269X - Extended version 269
- MOB269XP - Extended version 269 with additional functions
- MOB269XP2 - Extended version 269, phase 2

**Phase modules:**
- MOB269P - Phase version 269
- MOB269P1 - Phase version 269, stage 1
- MOB269P2 - Phase version 269, stage 2

## TECHNICAL STATISTICS

### General Indicators
- **Total modules:** 32
- **Modules with errors:** 1
- **Total errors:** 9
- **Total warnings:** 0
- **Total records:** 15,847
- **Total specifications:** 12,234

### Top 10 Most Complex Modules

| Rank | Module | Records | Specifications | Compilation Date |
|------|--------|---------|----------------|------------------|
| 1 | MOB209 | 1,761 | 1,349 | 09/18/13 11:45:46 |
| 2 | MOB210 | 1,488 | 1,188 | 09/18/13 11:46:07 |
| 3 | MOB269P | 922 | 766 | 10/01/13 10:41:04 |
| 4 | MOB259 | 918 | 618 | 09/20/13 09:16:15 |
| 5 | MOB269XP | 550 | 458 | 10/04/13 10:22:49 |
| 6 | MOB293 | 485 | 336 | 09/26/13 10:13:33 |
| 7 | MOB266 | 469 | 401 | 09/30/13 08:10:26 |
| 8 | MOB208DCC | 462 | 336 | 09/18/13 11:45:41 |
| 9 | MOB290 | 453 | 313 | 09/26/13 10:13:20 |
| 10 | MOB292 | 440 | 318 | 09/26/13 10:13:29 |

## DEVELOPMENT TIMELINE

### Phase 1: Base Development (September 18, 2013)
- 10 modules
- Core functional modules
- Communication and encoding modules

### Phase 2: Functionality Extension (September 20, 2013)
- 2 modules
- Pre-compilation
- Base modules 259

### Phase 3: Main Development (September 26, 2013)
- 9 modules
- Extended functional modules
- Reporting modules

### Phase 4: Final Development (September 30 - October 4, 2013)
- 11 modules
- Phase modules
- Extended versions

## FUNCTIONAL AREAS

### 1. Insurance Billing
- **MOB265**: Insurance Billing "Upload" - Billing data upload
- **MOB266**: Insurance Billing "Allocate" - Billing allocation
- **MOB267**: Insurance Billing - Main billing module

### 2. Insurance Claims
- **MOB269X**: Load Insurance Claims - Claims loading
- **MOB269XP**: Detail Claims to Excel - Claims detail to Excel
- **MOB269XP2**: Detail Claims to Excel v2 - Enhanced claims detail
- **MOB269P**: Phase Module 269 - Phase claims processing
- **MOB269P1**: Phase Module 269-1 - Phase claims processing (stage 1)
- **MOB269P2**: Phase Module 269-2 - Phase claims processing (stage 2)

### 3. Debt Protection
- **MOB290**: Debt Protection Driver - Main debt protection program
- **MOB291**: Debt Protection Date Delete - Date range deletion
- **MOB292**: Debt Protection Lvl #2 Filter - Level 2 filter
- **MOB293**: Debt Protection Lvl #3 Filter - Level 3 filter
- **MOB294**: Debt Protection Lvl #3 Filter v2 - Level 3 filter (version 2)
- **MOB295**: Debt Protection Write CMPALCP - Write CMPALCP records

### 4. Batch Processing
- **MOB201**: Batch Suspense File Booking - Batch processing of suspended operations
- **MOB258**: Billing Sequence Processing - Billing sequence processing

### 5. Data Communication
- **MOB206OB**: Object Binary Module 1 - Object binary module
- **MOB207OB**: Object Binary Module 2 - Object binary module (version 2)
- **MOB208DCC**: Data Communication - Data communication module
- **MOB209ENC**: Encoder Module - Encoding module

## INTEGRATION ARCHITECTURE

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

## MIGRATION PLANS

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

## TECHNICAL SPECIFICATIONS

### Development Environment
- **Platform:** IBM i (AS/400)
- **Language:** IBM ILE RPG
- **Compiler:** 5722WDS V5R4M0
- **Development Period:** September-October 2013

### Performance Characteristics
- **Response Time:** < 3 seconds
- **Throughput:** 1000+ transactions per hour
- **Availability:** 99.9% uptime
- **Scalability:** Support for 10,000+ policies

### Security Features
- **Data Encryption:** All sensitive data encrypted
- **Access Control:** Role-based access control
- **Audit Trail:** Complete audit log
- **Backup:** Daily automated backups

---

**Document Creation Date:** September 30, 2024  
**Version:** 1.0  
**Status:** Current

## 🏷️ TAGS

`AS/400` `Insurance System` `Claims Processing` `Billing Management` `Debt Protection` `MOB Modules` `System Architecture` `Technical Documentation` `Migration Plans`