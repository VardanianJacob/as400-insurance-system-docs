# AS/400 SYSTEM DOCUMENTATION (Insurance Claims & Billing System)

## 📋 OVERVIEW

Business documentation for AS/400 insurance policy and claims processing system. The system includes 32 MOB modules for managing insurance policies, claims, billing, and debt protection.

> **📖 Complete documentation index:** [INDEX.md](./INDEX.md)

## 📁 DOCUMENTATION STRUCTURE

### 🏗️ Main Documents

1. **[BUSINESS_DOCUMENTATION.md](./BUSINESS_DOCUMENTATION.md)** - Complete business documentation
   - System business processes
   - Description of all MOB modules
   - Integrations and reporting
   - Migration plans

2. **[MODULES_REFERENCE.md](./MODULES_REFERENCE.md)** - Modules reference
   - Complete list of 32 MOB modules
   - Detailed description of each module
   - Classification by categories
   - Statistics and migration plans

3. **[BRD_INSURANCE_SYSTEM.md](./BRD_INSURANCE_SYSTEM.md)** - Business requirements
   - System goals and objectives
   - Stakeholders
   - Success criteria
   - Requirements compliance

### 📊 Additional Files

4. **[PROJECT_DOCUMENTATION.md](./PROJECT_DOCUMENTATION.md)** - General project documentation
   - System architecture
   - Functional areas
   - Development timeline

5. **[MODULE_DOCUMENTATION.md](./MODULE_DOCUMENTATION.md)** - Detailed module documentation
   - Module technical specifications
   - Complexity statistics

6. **[SYSTEM_OVERVIEW.md](./SYSTEM_OVERVIEW.md)** - Brief system overview
   - Key characteristics
   - Status and plans
   - Key indicators

## 📁 SOURCE FILES

### Architectural Diagrams
- **[AS400ReplacementFlowChart.pdf](./AS400ReplacementFlowChart.pdf)** - System architecture diagram
- **[AS400 to FourPoint Export_Manual.pdf](./AS400%20to%20FourPoint%20Export_Manual.pdf)** - Data export manual

### Business Processes (Excel)
- **[DCC Coverage.xls](./DCC%20Coverage.xls)** - DCC coverage
- **[DCC New Business Process.xls](./DCC%20New%20Business%20Process.xls)** - New business process
- **[DCC Premium Allocation Process.xls](./DCC%20Premium%20Allocation%20Process.xls)** - Premium allocation process
- **[DCC Premium Process.xls](./DCC%20Premium%20Process.xls)** - Premium process
- **[Sovereign DCC Claims Export Process.xls](./Sovereign%20DCC%20Claims%20Export%20Process.xls)** - Claims export
- **[Sovereign DCC Premium Export Process.xls](./Sovereign%20DCC%20Premium%20Export%20Process.xls)** - Premium export
- **[Sovereign DCC Premium Import Process.xls](./Sovereign%20DCC%20Premium%20Import%20Process.xls)** - Premium import

### Technical Documentation
- **[Greg_s notes on Premium Allocation Processing.pdf](./Greg_s%20notes%20on%20Premium%20Allocation%20Processing.pdf)** - Premium processing notes
- **[as400 tables by pgm.xlsx](./as400%20tables%20by%20pgm.xlsx)** - AS/400 tables by programs
- **[iSeries Job Scheduler (2).xls](./iSeries%20Job%20Scheduler%20(2).xls)** - iSeries job scheduler

## 🚀 QUICK START

### Key Characteristics
- **System:** AS/400 (Insurance Claims & Billing System)
- **MOB Modules:** 32
- **Functionality:** Insurance policy and claims processing, billing, debt protection
- **Status:** In production (migration to C# planned)

### Functional Areas
- **Insurance Billing** - MOB265, MOB266, MOB267
- **Claims Processing** - MOB269X, MOB269XP, MOB269XP2
- **Debt Protection** - MOB290-295
- **Batch Processing** - MOB201, MOB258
- **Data Communication** - MOB206OB-209ENC

## 📚 USING THE DOCUMENTATION

### For Business Users
1. Start with [BUSINESS_DOCUMENTATION.md](./BUSINESS_DOCUMENTATION.md) to understand processes
2. Use [MODULES_REFERENCE.md](./MODULES_REFERENCE.md) as a module reference
3. Study [BRD_INSURANCE_SYSTEM.md](./BRD_INSURANCE_SYSTEM.md) to understand requirements

### For Analysts
1. Use [MODULES_REFERENCE.md](./MODULES_REFERENCE.md) for functionality analysis
2. Refer to [PROJECT_DOCUMENTATION.md](./PROJECT_DOCUMENTATION.md) for architecture
3. Study migration plans in business documentation

## ⚠️ IMPORTANT INFORMATION

### Migration Plans
- **AS/400 marked as "Decommissioned long ago"**
- **Planned replacement of Debt Protection modules (MOB290-295) with C# Window Service**
- **Other modules continue to run on AS/400**

---

**Documentation creation date:** September 30, 2024  
**Version:** 1.0  
**Status:** Current

## 🏷️ TAGS

`AS/400` `Insurance System` `Claims Processing` `Billing Management` `Debt Protection` `MOB Modules` `Business Documentation`