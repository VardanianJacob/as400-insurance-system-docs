# AS/400 Insurance Claims & Billing System Documentation

[![Documentation Status](https://img.shields.io/badge/Documentation-Complete-green.svg)](./INDEX.md)
[![System Status](https://img.shields.io/badge/System-In%20Production-blue.svg)](./SYSTEM_OVERVIEW.md)
[![Migration Status](https://img.shields.io/badge/Migration-Planned-yellow.svg)](./BUSINESS_DOCUMENTATION.md)

## 📋 Overview

This repository contains comprehensive business documentation for the AS/400 Insurance Claims & Billing System. The system includes 32 MOB modules for managing insurance policies, claims, billing, and debt protection.

## 🏗️ System Architecture

- **Platform:** AS/400 (IBM i)
- **Language:** IBM ILE RPG
- **Modules:** 32 MOB modules
- **Status:** In production (C# migration planned)
- **Functionality:** Insurance policy and claims processing, billing management, debt protection

## 📁 Documentation Structure

### 📖 Main Documents

- **[INDEX.md](./INDEX.md)** - Complete documentation index
- **[BUSINESS_DOCUMENTATION.md](./BUSINESS_DOCUMENTATION.md)** - **MAIN DOCUMENT** - Business processes and modules
- **[MODULES_REFERENCE.md](./MODULES_REFERENCE.md)** - **MODULE REFERENCE** - Detailed module descriptions
- **[BRD_INSURANCE_SYSTEM.md](./BRD_INSURANCE_SYSTEM.md)** - Business requirements document

### 📊 Additional Documents

- **[PROJECT_DOCUMENTATION.md](./PROJECT_DOCUMENTATION.md)** - Project overview and architecture
- **[MODULE_DOCUMENTATION.md](./MODULE_DOCUMENTATION.md)** - Technical module details
- **[SYSTEM_OVERVIEW.md](./SYSTEM_OVERVIEW.md)** - System summary and key metrics

## 🎯 Quick Start

### For Business Users
1. Start with [BUSINESS_DOCUMENTATION.md](./BUSINESS_DOCUMENTATION.md) for process understanding
2. Use [MODULES_REFERENCE.md](./MODULES_REFERENCE.md) as module reference
3. Review [BRD_INSURANCE_SYSTEM.md](./BRD_INSURANCE_SYSTEM.md) for requirements

### For Analysts
1. Review [BRD_INSURANCE_SYSTEM.md](./BRD_INSURANCE_SYSTEM.md) for business requirements
2. Study [BUSINESS_DOCUMENTATION.md](./BUSINESS_DOCUMENTATION.md) for processes and modules
3. Check [PROJECT_DOCUMENTATION.md](./PROJECT_DOCUMENTATION.md) for architecture

## 🏦 Business Processes

### Core Functions
- **Policy Management** - Creation, modification, renewal of insurance policies
- **Claims Processing** - Registration, investigation, settlement of insurance claims
- **Billing Management** - Invoice generation, payment processing, debt management
- **Debt Protection** - Risk assessment, debt collection, financial protection

### Key Modules
- **Insurance Billing** - MOB265, MOB266, MOB267
- **Insurance Claims** - MOB269X, MOB269XP, MOB269XP2
- **Debt Protection** - MOB290-295
- **Batch Processing** - MOB201, MOB258
- **Data Communication** - MOB206OB-209ENC

## ⚠️ Migration Status

### Current Status
- **AS/400 system** marked as "Decommissioned long ago"
- **Debt Protection modules (MOB290-295)** planned for replacement with C# Window Service
- **Other modules** continue to operate on AS/400

### Planned Changes
- **C# Window Service** will replace Debt Protection modules
- **Functions:** FTP monitoring, certificate validation, value checking, data matching
- **Timeline:** To be determined

## 📊 System Statistics

- **Total Modules:** 32 MOB modules
- **Code Records:** 15,847
- **Compilation Errors:** 9 (0.28%)
- **Comment Coverage:** 4.8%
- **Development Period:** September-October 2013

## 🔧 Technical Details

### Platform Requirements
- **OS:** IBM i 7.1 or higher
- **Processor:** PowerPC 64-bit
- **Memory:** Minimum 4 GB RAM
- **Compiler:** 5722WDS V5R4M0

### Integration Points
- **Four Point (Java/Oracle)** - Main system
- **FTP Server** - File exchange
- **apsPlateau Database** - Corporate database
- **BreakDown Values** - Reference data

## 📈 Business Value

### Key Benefits
- ✅ **Process Automation** - Streamlined insurance operations
- ✅ **Error Reduction** - Automated validation and processing
- ✅ **Efficiency Improvement** - Faster claim and billing processing
- ✅ **Compliance** - Regulatory requirements adherence

### Success Metrics
- **Claims Processing Time:** < 24 hours
- **Billing Accuracy:** > 99.5%
- **System Availability:** > 99.9%
- **Response Time:** < 3 seconds

## 📞 Support

### Documentation
- **Complete business documentation** available in this repository
- **Module reference** for all 32 MOB modules
- **Process flows** and integration details

### Contact
- **Technical Support:** 24/7 monitoring
- **Response Time:** 4 hours
- **Documentation:** Full technical documentation available

## 📄 License

This project is developed for internal use. All rights reserved.

---

**Documentation Created:** September 30, 2024  
**Version:** 1.0  
**Status:** Current  
**Next Review:** December 30, 2024

## 🏷️ Tags

`AS/400` `Insurance System` `Claims Processing` `Billing Management` `Debt Protection` `MOB Modules` `Business Documentation` `Legacy System` `Migration` `C#` `RPG` `IBM i`
